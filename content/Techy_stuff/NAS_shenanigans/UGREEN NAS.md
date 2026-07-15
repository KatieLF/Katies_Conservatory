---
title: UGREEN NAS
draft: false
---

### Backstory

While the concept of a Network Attached Storage device was still quite new to me, my father purchased two for the family. My fiancé (then my boyfriend) had mentioned the idea to him a few times and Dad thought it would be the best way to preserve the family's digital assets (photos, files, burned CDs, and the like). Now, I love my father deeply, and he has spearheaded much of our family's digital infrastructure, but this was just a liiiittttlllleeee too out of his wheelhouse. So in an attempt to learn how to setup infrastructure for users, I volunteered myself as tech support.

The new users struggle has been [well documented](https://uncarafedeausilvousplait.github.io/Ugreen-Annoyance/), so I want to emphasize again, NAS's are AMAZING machines and a giant step towards [[[Ownership]]], they also requires a lot of technical knowhow or the willingness to learn.

### Infrastructure

My family's main needs are media, photos, and files.

- [[JellyFin]]
  The media angle was more my idea. It was cheaper to get the disk then it was to take 4 kids to the movies so we have a WALL of DVDs and Blu-rays. My Christmas gift to my father (once he got the NAS) was to digitize the collection. I used [Jellyfin](https://jellyfin.org/) to make it easily accessible and my "users" didn't have to mess around with files. While UGREEN does have a Jellyfin app in their app store, after a bit of research I learned it was not updated often and you couldn't customize the settings. Thankfully, Jellyfin's documentation is pretty stellar and I was able to get the server up and running within a day using their docker compose file. Since I want my family to be able to add their own media to the server, I made the db for the files within the shared folders of the family.
  PICTURE HERE

- [[Immich]]
  Photos is one of the main reasons my father decided on a NAS. The iOS Photos app ended up losing some of our family memories and their help line said "oh well!"
  This is still not fully implemented as the user sharing is limited. I hope to contribute to the [Immich project](https://immich.app/)to make the sharing more multi user friend (or make an extension? idk that's a ways in the future. )

- [[Tailscale]]
  The great, the amazing, the stupendous! [Tailscale](https://tailscale.com/). This is the magical tool that connects everything together outside of the home WIFI network. While technically an enterprise tool, it allows a free version that is perfect for home labs. As long as your connected to the tailnet, you're connected to everything.
