---
title: JellyFin
draft: true
---

Since Jellyfin has been so beloved by the community, there is a TON of documentation about how to set everything up. At first I started with the UGREEN app (don't recommend), but then I found I could still host Jellyfin via Docker.

IMG HERE APP STORE JELLYFIN

After some finagling of where I wanted the actual files to go, I booted it up on docker.

IMAGE HERE OF DOCKER COMPOSE FILE

It currently eats up a third of 8gb of ram that I have and I have not stress tested it as of yet (i.e. having everyone stream something at the same time).

IMG OF HARDWARE USAGE OF JELLYFIN

1 main downside that I recently noticed is downloading on the mobile app. The Jellyfin app will allow you to download the media, but it can't be played through the app. You just download the file and then need another application like VLC to play the file. Not entirely sure why it's built this way. Again, hopefully in a few years I will be able to make an extension or contribute to Jellyfin to fix this little ick of mine.

IMG OF DOWNLOADS ON MOBILE
