# Crizzy Development — public site

Static pages served by GitHub Pages at <https://apps.crizzy.ca>. This repository exists to
host the privacy policy and support page that each published app is required to link to, on a
public URL that does not depend on any app repository being public.

**This repository is public and so is its history.** Nothing but the site belongs in it.

## Layout

```
index.html              the app list
404.html
CNAME                   apps.crizzy.ca
.nojekyll               served as-is; no Jekyll build
assets/site.css         shared styling
<app>/index.html        one directory per app
<app>/privacy/index.html
<app>/support/index.html
```

Directories, not `.html` files, so the published URLs carry no extension and can be changed
later without breaking a link printed in a store listing. Adding an app is a new directory.

## The one rule

**A privacy policy has to stay reachable.** Google Play requires the URL on a listing to be
live, public, non-geofenced and specific to the app; a link that dies is a policy violation
rather than a broken page. Do not rename or move a directory that a published listing points
at — add a new one and leave the old one in place.
