---
layout: default
title: "About Pixel In Waiting"
---

# About Pixel In Waiting

## Why

My friend and I were tracking games we wanted to play in a Google Sheet. It worked, but typing everything in by hand was tedious, and on a phone it was basically a tiny spreadsheet you had to pinch and zoom around. Other game trackers exist, but many are built around accounts, ads or subscriptions. I wanted something minimal that kept my data mine, with a few quality-of-life improvements.

## How

The app pulls game data from Wikidata using just your search text (shout out to Wikidata for their free, anonymous endpoints). Covers, time to beat and ratings come from IGDB, through a small server of mine that looks up games by ID so the access key stays off your phone. Your library lives on your devices and iCloud keeps them in sync. Sharing with friends is iCloud too, so my server is never in the middle of your library or your friends. Friends only see what you choose to share, and the rest stays yours. You can export it any time to take it somewhere else, or delete it and forget about it. If you turn on release-day reminders, they are made on your phone or Mac too; nothing about them leaves it.

Because the app is free, the first launch had no servers of mine, which limited features like artwork, longer game details and popularity. Now there is one small server, on Cloudflare's free plan, that fetches those from IGDB. It keeps nothing about you.

## Future

IGDB is hooked up now, for richer game information. That is my first server, since it needs credentials and rate limiting. I think I can run it for little or no cost unless the app somehow becomes popular. If hosting ever costs me too much, that's where I might add something paid, and I'd be upfront about it, with the price tied to what it costs me to keep the app running.

Syncing from game stores would be a nice long-term addition, but from what I can tell most of that data is closed off. For now, the way to bring in your games is to import whatever you can export from your game store. I won't skirt store rules, so neither of us risks a ban.

Have an idea for a feature? Email me (the address is on the [Support](../support/) page). I'll check whether it would cost anything to host or to get access to other systems before I say yes. If it does, it would either wait or go in a paid tier.

## About me

My friend and I like playing games together, whether that's co-op online or single-player games played at the same time so we can chat about them. I built this so we could share our games and pick what comes next. If nobody else uses it, that's okay.

I built it with Claude's help to speed up the writing, but I made the architecture choices and set the direction. That's how I kept costs at zero (yes, it wanted to use cloud resources right out of the gate) and made sure your data stays yours. When the App Store first launched, it was fun to find free new apps that did small things and didn't need to be online. I couldn't keep this one completely offline. Game info comes from Wikidata and IGDB, and syncing and sharing run on iCloud. Your library still works without a connection, and I kept everything else bare-bones like the good old days.

[Back to Pixel In Waiting](../)
