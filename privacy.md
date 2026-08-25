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

     Also: if you ever add analytics, this page must change the same day.
     --------------------------------------------------------------------- -->

{% if site.gtm_id and site.gtm_id != "" %}
This site is a set of files. It has no accounts, no comments and no advertising.
The typefaces are served from this site rather than from Google, and there are
no embedded videos, share buttons or fonts loaded from elsewhere.

It does, however, measure visits.

## Analytics

I use Google Tag Manager and, through it, Google Analytics, to understand how
many people read these pages and which ones they read. This means Google
receives information about your visit: your IP address, the pages you look at,
roughly where in the world you are, and what browser you use.

I use it to answer questions like *did anyone read that post* and *are people
finding the book*. I don't use it to identify individuals, and I have no way of
doing so.

{% if site.gtm_consent_default_denied %}If you are reading this from the
European Economic Area, the United Kingdom or Switzerland, nothing is stored on
your device unless you consent to it — no analytics cookies are set, and what
measurement happens is anonymous and aggregated. Elsewhere, including Australia,
Google Analytics sets a cookie to recognise a repeat visit. No advertising
cookies are set anywhere, and nothing here is used for advertising.{% else %}
Google Analytics sets cookies in your browser to recognise a repeat visit.{% endif %}

If you'd rather not be counted, any of these will prevent it: a browser with
tracking protection on (Safari and Firefox do this by default), an ad blocker,
Chrome's Do Not Track setting, or Google's own
[opt-out browser add-on](https://tools.google.com/dlpage/gaoptout). None of them
affect your ability to read anything here.

Google's handling of the data is governed by their own privacy policy, not mine.
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
