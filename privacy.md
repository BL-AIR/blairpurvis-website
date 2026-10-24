---
title: Privacy
permalink: /privacy/
standfirst: >-
  What this site collects, which is very close to nothing.
description: Privacy statement for blairpurvis.com.
---

<!-- ---------------------------------------------------------------------
     A note to you, not to readers.

     I am not a lawyer and this is not legal advice. What follows is an
     honest, plain-English description of what the site actually does —
     which is the most important quality a privacy statement can have,
     because an inaccurate one is worse than none.

     It is accurate as the site stands today. Two things will change it:

     1. Switching on the mailing list. The relevant section below is
        already written but commented out — uncomment it and name the
        provider.
     2. Switching on the contact form. Same.

     Also: if you ever add a new tracking tool, this page and the cookie
     table below must change the same day, and VERSION in
     assets/js/consent.js must go up by one.
     --------------------------------------------------------------------- -->

{% if site.gtm_id and site.gtm_id != "" %}
This site is a set of files. It has no accounts, no comments and no advertising.
The typefaces are served from this site rather than from Google, and there are
no embedded videos, share buttons or fonts loaded from elsewhere.

It does, however, measure visits — but only if you say so.

## Analytics

With your permission, I use Google Tag Manager and, through it, Google
Analytics, to understand how many people read these pages and which ones they
read. Google then receives information about your visit: your IP address, the
pages you look at, roughly where in the world you are, and what browser you use.

Also with your permission, I use Microsoft Clarity, which records how pages are
used — clicks, scrolling, how far down a post people read — so I can see what
works and what doesn't. Clarity masks anything typed into a form and doesn't
collect names or contact details.

I use these to answer questions like *did anyone read that post* and *are
people finding the book*. I don't use them to identify individuals, and I have
no way of doing so.

If you decline, Clarity doesn't run at all, and Google Analytics receives only
an anonymous signal that a page was viewed — no cookie, and nothing that links
one visit to the next. Nothing here is used for advertising.

Google's and Microsoft's handling of the data is governed by their own privacy
policies, not mine.

## Cookies {#cookies}

Cookies are small files a website stores in your browser. The first time you
visit, a small panel asks which kinds you allow, and nothing optional runs
until you choose. You can change your mind at any time with
<a href="{{ '/privacy/#cookies' | relative_url }}" data-cookie-settings>Cookie settings</a>,
at the foot of every page. I ask again after 12 months, or sooner if I add a
new tool.

| Category | Tool | What it stores | How long |
| --- | --- | --- | --- |
| Essential (always on) | This site | Your cookie choice, kept in your browser only | 12 months |
| Statistics | Google Analytics (`_ga`, `_ga_*`) | A random ID that tells one visit from the next | Up to 2 years |
| Statistics | Microsoft Clarity (`_clck`, `_clsk`) | A random ID linking the pages of one visit | Up to 1 year |
| Marketing | None at present | — | — |

You can also block or delete cookies in your browser settings. Everything here
can be read without optional cookies.
{% else %}
This site is a set of files. It has no accounts, no comments, no advertising,
and no analytics. It sets no cookies and stores nothing in your browser.

It also makes no requests to anyone else. The typefaces are served from this
site rather than from Google, and there are no embedded videos, share buttons,
tracking pixels or fonts loaded from elsewhere. Visiting these pages does not
tell any third party that you were here.
{% endif %}

## What the host sees

The site is hosted by GitHub Pages. Like every web server, GitHub's receives
the ordinary information your browser sends in order to deliver a page: your
IP address, the page you asked for, the time, and your browser type. GitHub
uses this to serve the site and to defend it against attack. I have no access
to those logs and no ability to identify you from them. GitHub's own privacy
statement covers what they do with it.

## If you write to me

If you send an email to <me@blairpurvis.com>, your message and address arrive
in my mailbox, which is hosted by Zoho. I read it, I may reply, and it stays
in my mail like any other correspondence. I don't add you to anything, pass
your address to anyone, or use it for any purpose other than answering you.

<!-- ---------------------------------------------------------------------
     UNCOMMENT WHEN THE MAILING LIST IS SWITCHED ON, and replace
     [PROVIDER] with whoever runs it.

## The mailing list

If you join the mailing list, you give me your name and your email address.
They are held by [PROVIDER], who deliver the mail, and are used for one
thing: sending you a few notes a year about the books. They are never sold,
never traded, and never passed to anyone else.

Every message includes a link to leave, which removes you immediately and
permanently. You can also ask me directly and I'll do it by hand.
     --------------------------------------------------------------------- -->

<!-- ---------------------------------------------------------------------
     UNCOMMENT WHEN THE CONTACT FORM IS SWITCHED ON.

## The contact form

The contact form sends me your name, your email address and your message.
It is delivered to my mailbox and stored nowhere else — there is no database
behind this site. The information is used to reply to you and for nothing
else.
     --------------------------------------------------------------------- -->

## Your rights

If you're in Australia, the UK, the European Union, or anywhere with similar
laws, you have the right to ask what information I hold about you, to have it
corrected, and to have it deleted. Write to me and I'll do it. Given how little
there is, this is usually a short conversation.

## Children

Nothing here is directed at children, and I don't knowingly collect anything
from anyone under the age required by their local law.

## Changes

If this site ever starts doing something it doesn't do today — analytics, a
mailing list, a form — this page will be updated to say so before that happens,
not after. It's kept in the same repository as the site itself, so its history
is a matter of public record.

## Who to ask

Blair Purvis — <me@blairpurvis.com>

Published by [Prahran Publishing]({{ site.publisher.url }}), Melbourne, Australia.

*Last updated {{ 'now' | date: "%-d %B %Y" }}.*
