# Site setup: analytics and reader signup

Two small things, both already in place and both **inert until you finish them**,
so nothing broken is showing in the meantime. Do them in either order; the
analytics one is faster and answers the readership question on its own.

---

# Part A. Cloudflare Web Analytics

This tells you how many people read the book, which countries they are in, which
chapters they open, and who is linking to you. No cookies, no personal data, no
consent banner needed.

## A1. Make the account

Go to **dash.cloudflare.com** and sign up. Free. You do **not** need to move your
domain to Cloudflare or change any DNS; the beacon works on GitHub Pages as it is.

## A2. Add the site

In the left sidebar find **Analytics & Logs → Web Analytics**, then
**Add a site**. Enter:

```
aigov.ogunseye.com
```

Cloudflare shows you a snippet containing a long token, something like:

```
data-cf-beacon='{"token": "a1b2c3d4e5f6..."}'
```

Copy **just the token**, the part between the quotes after `"token":`. Not the
whole snippet.

## A3. Paste it in

Open `analytics.html` and find this line:

```
var TOKEN = "PASTE_CLOUDFLARE_TOKEN_HERE";
```

Replace the placeholder with your token, keeping the quotes.

## A4. Render and push

```
quarto render --to html
git add docs analytics.html _quarto.yml
git commit -m "Add Cloudflare Web Analytics"
git push
```

Data starts appearing within a few minutes of the first visit. Give it a day
before reading anything into it.

---

# Part B. Reader signup

The widget is already on the landing page and is **hidden until you do this**, so
nothing broken is showing in the meantime.

It posts to a Google Form exactly the way the chapter feedback widget does, so
responses land in a Google Sheet you already know how to read.

## B1. Make the form

Google Forms, blank form. Title it whatever you like; readers never see it.

Add **three short-answer questions, in this order**:

| # | Question text | Required? |
|---|---|---|
| 1 | Name | no |
| 2 | Email | no |
| 3 | Role or institution | no |

Leave them all optional. The widget does its own checking before it sends, and a
required field on Google's side will silently reject the submission.

Then **Responses → link to Sheets** so they collect somewhere you can read.

## B2. Get the four values

**The form action URL.** Click Send, choose the link icon, copy the URL. It ends
in `/viewform`. Change that last part to `/formResponse`. That is the value for
`FORM_ACTION`.

**The three entry IDs.** This is the fiddly bit and there is an easy way:

1. In the form editor, click the three dots at the top right
2. Choose **Get pre-filled link**
3. Type `NAME` in the first box, `EMAIL` in the second, `ROLE` in the third
4. Click **Get link**, then **Copy link**
5. Paste it somewhere you can read it

The pasted URL contains something like:

```
entry.123456789=NAME&entry.987654321=EMAIL&entry.555555555=ROLE
```

The number next to `NAME` is your `ENTRY_NAME`, and so on.

## B3. Paste them in

Open `_signup-widget.qmd` and find these four lines near the bottom:

```
var FORM_ACTION  = "PASTE_FORM_ACTION_URL_HERE";
var ENTRY_NAME   = "entry.PASTE_NAME_ID";
var ENTRY_EMAIL  = "entry.PASTE_EMAIL_ID";
var ENTRY_ROLE   = "entry.PASTE_ROLE_ID";
```

Replace each placeholder, keeping the quotes and keeping the `entry.` prefix on
the three IDs.

## B4. Render and push

```
quarto render --to html
git add docs index.qmd _signup-widget.qmd
git commit -m "Wire up reader signup"
git push
```

The widget appears once `FORM_ACTION` no longer starts with `PASTE_`.

## B5. Test it

Load the landing page, send yourself a test entry, and check it arrives in the
Sheet. If nothing arrives, the usual cause is a required question on the Google
side, or an entry ID pasted without its `entry.` prefix.

## Taking it down

Delete the `{{< include _signup-widget.qmd >}}` line from `index.qmd` and delete
`_signup-widget.qmd`. Nothing else refers to either.

## What you promised the reader

The widget says, in the reader's sight: the three fields and the date are
collected, they are used to tell people when the book changes, they are not
shared or sold, and they are deleted on request or when this edition is
superseded. If you later use the list for something else, change the text first.
