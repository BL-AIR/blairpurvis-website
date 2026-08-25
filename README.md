# blairpurvis.com

A Jekyll site, hosted free on GitHub Pages. No database, no CMS, no logins,
no monthly bill. Files in, website out.

---

## Publishing a blog post

1. Make a new file in the `_posts` folder.
2. Name it `YYYY-MM-DD-some-words.md` — the date is how Jekyll orders posts,
   and the words become the web address.
3. Start the file with this block, between the two lines of dashes:

```
---
title: What the post is called
date: 2026-09-01 10:00:00 +1000
standfirst: One sentence that appears under the title and in the list.
---
```

4. Write underneath it, in plain markdown. A blank line between paragraphs.
   `*italics*`, `**bold**`, `### a subheading`, `[a link](https://example.com)`.
5. Save. Commit and push with GitHub Desktop.

It's live in about a minute. That's the whole system.

**To hold something back:** add `published: false` as its own line inside the
front matter block. The file stays in the repository; the post doesn't appear
anywhere. Delete that line when you're ready.

Two of the 2018 posts are held back this way — see the note at the top of each.

---

## Changing things without touching code

Almost everything lives in **`_config.yml`**:

| What | Where |
|---|---|
| Site description, your name, your email | top of `_config.yml` |
| Which social accounts appear | `social:` — delete a line to remove a link |
| The mailing list promise | `mailing_list_promise:` |
| Turning the mailing list on | `mailing_list_action:` — paste the provider's URL |
| Turning the contact form on | `form_endpoint:` — paste the Worker's URL |

While `mailing_list_action` and `form_endpoint` are empty, those sections show
a plain email link instead. Nothing is broken and nothing silently swallows a
message. Fill either one in and the form appears by itself.

**Books** live in `_data/books.yml`. Add a book by copying an existing block.
Buy links are commented out until you have them — a missing link is better
than a dead one.

**Pages** — `about.md`, `press.html`, `contact.html` — are ordinary files.
Edit the words, push, done.

---

## Pictures

Put them in `assets/img/` and refer to them by filename.

Before you publish any photograph, **strip the EXIF data**. Camera files carry
GPS coordinates, and a portrait taken at home is a portrait that publishes your
address. On a Mac: open in Preview → Tools → Show Inspector → the (i) tab →
remove location info. Or ask me and I'll do a batch.

Every image needs alt text — a plain description of what's in it, for people
using screen readers and for anyone whose connection drops the image.

---

## Going live

1. Create a repository on GitHub and push this folder to it.
2. Repository → Settings → Pages → Source: deploy from branch `main`, folder `/`.
3. Settings → Pages → Custom domain: `blairpurvis.com`. Tick **Enforce HTTPS**
   once the certificate is issued (can take an hour).
4. In GoDaddy's DNS for `blairpurvis.com`:

   **Replace** the two A records with GitHub's four:

   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

   **Add** a CNAME: `www` → `bl-air.github.io`

   > **Leave the MX and TXT records completely alone.** They carry your Zoho
   > mail. Deleting them stops `me@blairpurvis.com` receiving anything, and it
   > fails silently — you don't find out, the sender doesn't find out.

---

## Running it on your own machine first (optional)

```
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`. Changes appear as you save. Useful for
checking a post reads properly before it's public, though pushing straight to
GitHub is perfectly safe too.

---

## What's where

```
_config.yml          settings — start here
_data/books.yml      the books
_posts/              blog posts, one file each
_layouts/            page templates
_includes/           header, footer, mailing list block
assets/css/main.css  all the styling; colours are named at the top
assets/img/          photographs and cover art
index.html           the front page
about.md             the long bio
books.html           the books page
writing.html         the blog index
press.html           the press kit
contact.html         the contact page
CNAME                tells GitHub the domain is blairpurvis.com — don't delete
```

---

## If something looks wrong

The site builds on every push. If a build fails, GitHub emails you and the
site keeps serving the last good version — you can't break it into a blank
page by pushing a bad file.

Most build failures are a mistake in the front matter block: a missing dash
line, or a colon inside a title that isn't wrapped in quotes. Titles with
colons need quotes: `title: "Chapter One: Morocco"`.
