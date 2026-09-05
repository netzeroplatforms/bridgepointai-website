# BridgePoint AI website

**The public website lives in `/docs`. Only `/docs` is published.**

Anything outside that folder is in the repository but is NOT a public address.
That is deliberate, and it is the fix for what happened on 5 September 2026.

## What happened, so it does not happen again

GitHub Pages used to publish the **root** of this repository. Every file
committed here became a live URL on www.bridgepointai.io - immediately, silently,
with no warning and no link needed to find it.

Client draft work ended up public that way: a draft HH Global site with named
profile pages, three HeartsSight drafts including one on Class IIa regulatory
positioning, and a page of CityFi outreach templates carrying a working email
address. None of it was linked from the site. All of it was readable by anyone.

**Unlinked is not private. It is only undiscovered.**

## The rules, set by Mark and Virginia, 5 September 2026

1. **Documents we produce - forecasts, one-pagers, valuations, business plans,
   call briefs - are made as PDFs and held in the document library**, in the
   folder for that client. They do not go in a website repository, ever, not
   even briefly, not even in a subfolder.

2. **The document library is behind Cloudflare Access.** That is a login, not an
   obscure address. An unguessable URL protects nothing.

3. **`robots.txt` is not access control.** It asks search engines politely and
   stops nobody else, and a `Disallow` line publishes the very path you are
   trying to hide.

4. **A draft for review does not go on a public host.** If a client needs to see
   it, put it behind the Access gate and send them the link.

## If you are adding a page to the actual website

Put it in `/docs`. Check it is linked from somewhere. Then it is a website page,
which is the only thing this repository should publish.

## Monitoring

Selected addresses on this site are checked daily by
`agents/virginia/scripts/exposure-check.py`. It is silent when everything is as
expected and complains loudly when it is not.
