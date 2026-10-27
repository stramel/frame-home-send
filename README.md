# Send to Frame Home

The page your phone opens when you scan the code on Frame Home's
**Settings › Art › Add your images › From your phone** screen.

It sends the photos you pick, at full size and quality (HEIC becomes a full-resolution JPEG,
since the TV can't show HEIC), to the TV owner's own Frame Home photo relay: a small
Cloudflare Worker, set up from `relay/` in the Frame Home project. The link's `#t=` is the
TV's secret mailbox code and `#r=` the relay's address; the part after `#` never reaches
GitHub. The relay keeps each photo only until the TV has saved it. This page holds no keys and stores nothing.

Published with GitHub Pages at https://stramel.github.io/frame-home-send/.
