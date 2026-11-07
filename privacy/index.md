---
layout: default
title: "Pixel In Waiting — Privacy Policy"
---

# Pixel In Waiting — Privacy Policy

_Effective 2026-11-05_

Pixel In Waiting is an app for Mac and iPhone that tracks video games you have played or want
to play. It is made by Nate Rowan, one person. This page says what happens to your data.

**The short version:** your game list belongs to you. The developer has no accounts, no
analytics and keeps no copy of your library, notes or ratings. To show covers and game
details, the developer runs a small Cloudflare Worker that passes the app's requests on to IGDB.
It keeps no record of them.

## What the app stores

- **Your library:** the games you add and what you record about them (status, rating,
  interest, notes such as *Why Play It* and *My Review*, dates, platform played).
- **Your settings and friends list** on your device.
- **Copies of your friends' libraries,** on your device only, so you can browse them offline.
  They are replaced when a friend stops sharing and are removed when you remove the friend.
- **A short log of sharing events** (such as an invite sent or accepted, with times, counts and
  shortened IDs, and friends' names), on your device only. It is shown in TestFlight builds and
  never leaves your device unless you send it (see **Support info**).
- **A short history of removals, imports and changes,** on your device only, for undoing them
  for three days.
- **Game facts and pictures from IGDB,** on your device only: covers, screenshots, time to
  beat, game modes and ratings, kept so the app works offline and doesn't ask twice. They are
  never synced, exported or shared. **Settings ▸ Game Data ▸ Clear Cached Game Data** removes them.

On your device this is kept in the app's own storage. When iCloud sync is available, your
library is also kept in **your own iCloud account** (Apple's CloudKit), so it can appear on
your other devices. It is stored in your private iCloud and counts against your iCloud
storage. The developer cannot read it; only your devices and the people you choose to share
with (see below) can.

Next to your library, your private iCloud also keeps two facts about each game, taken from IGDB:
the main story time and the game modes. That lets your other devices show them without asking
again. They are kept apart from the library you share, so friends cannot see them. You can turn
this off in **Settings ▸ Game Data**, and Delete All My Data removes them.

## What the app sends over the internet

- **Game search and details:** when you search for a game or open its details, the app asks
  [Wikidata](https://www.wikidata.org) (run by the Wikimedia Foundation). The search text and
  the game's ID are sent, and Wikidata, like any website, sees your device's IP address. The
  app also tells Wikidata its own name and version, as Wikimedia's rules require. No name,
  account or library is sent. See the
  [Wikimedia Foundation Privacy Policy](https://foundation.wikimedia.org/wiki/Policy:Privacy_policy).
- **Game details, covers and lists (IGDB):** [IGDB](https://www.igdb.com) is a game database
  owned by Twitch. When the app needs a game's cover, time to beat, modes or ratings, it asks a
  small server run by the developer (hosted by Cloudflare), by the game's ID or web name. This
  happens for the games in your library when the app opens, for a game you open, and for the
  games shown in Add a Game's lists, in search results and in a friend's library. The server
  passes the question on to IGDB with the developer's own access key and sends the answer back.
  **Not sent:** the words you search for (searching stays with Wikidata), your name, your
  account, your notes, ratings or play status. The request also carries a key that is the same in
  every copy of that kind of build (it says "this is the app", not who you are). The server's
  host, like any website, sees your device's IP address. The server keeps **no log of requests**.
  To stop abuse it keeps a running count of requests per network address for up to an hour, and
  a once-a-day copy of the popular and upcoming games lists, which belongs to no one.
- **Pictures:** covers and screenshots are downloaded straight from IGDB's image servers, which,
  like any website, see your IP address and which picture you asked for.
- **Links you open:** buttons such as *Where to Buy* open a store or reference website in
  your browser. Those sites have their own privacy policies, and the app sends them nothing
  but the address you opened.
- **iCloud:** syncing and sharing go through Apple's iCloud under Apple's own terms and
  [privacy policy](https://www.apple.com/legal/privacy/).
- **Notifications from iCloud:** so your devices hear about changes without being opened, the
  app asks Apple to send it a silent notification when your library or a friend's library
  changes. It carries no content, shows nothing on screen and goes through Apple's push
  service. The developer receives nothing.

That is everything. There are **no ads, no analytics, no tracking and no third-party
software** that collects data about you.

## Sharing with friends

When friend sharing is turned on, you choose who can see your library. A friend you share
with can see **your whole library, including your notes and reviews**, and can add a game to
it. The app does not let them change or delete anything. (iCloud gives an invited friend
write access to your shared library, so this limit is kept by the app, not by iCloud.) You
can stop at any time: **removing a friend
removes the link between you on both sides and deletes each person's copy of the other's
library.** Your own library is not touched. Only share with people you are happy to show
your list to.

To invite someone, the app asks Apple's iCloud for a private invite link and hands it to
Apple's share panel (Messages, Mail or Copy Link). The link only works for the person you
invited. The name you choose for yourself (your profile name) is stored in your iCloud and
shown to people you share with. Until someone accepts, you see them as "Invited friend" or
the name Apple gives. When a friend adds a game to your library, their profile name is saved on
that game ("Added by") and shown to you.

## Your choices

- **Export:** you can export your library (CSV or JSON) whenever you like, so your data can
  always leave.
- **Delete:** you can remove games one by one, or delete all your data in the app: on iPhone
  in **Home ▸ Settings (the gear) ▸ Delete All My Data**, and on Mac in **Settings ▸ Delete All My Data** or **File ▸ Delete All My Data**.
  That removes your library, history, friends and settings from this device, and, once iCloud
  sync is on, your games and your profile name from your iCloud copy. It also ends your sharing,
  so the friends you shared with can no longer see your games. It can't be undone.
- **Stop sharing** with a friend whenever you want.
- **Support info:** if something goes wrong, **Settings ▸ Support Info** shows a short report you can
  read, copy or share to get help. It is made on your device and goes nowhere unless you send it.
  It holds the app and system versions, the iCloud status, counts and a log of sharing events with
  their times. Names are replaced with "Me" and "Friend 1", "Friend 2", links and email addresses are
  removed, and long numbers and iCloud IDs are cut short.
- You can also delete the app's iCloud data in your device's iCloud settings.

## TestFlight and the App Store

If you install through TestFlight or the App Store, **Apple** may collect crash reports,
usage and feedback you choose to send, under Apple's terms. The developer receives only what
Apple provides, such as crash logs and any feedback you send through TestFlight.

TestFlight builds also have **iCloud Diagnostics** in Settings, a troubleshooting screen with
more detail than Support Info, including friends' names and the invite link. You can copy it
to send to the developer; it goes nowhere unless you do. The App Store version does not have
it. The app asks Apple whether it was installed through TestFlight or the App Store to decide
this, and sends nothing else.

## Children

The app is not directed at children and does not knowingly collect anything from them.

## Changes

If the app starts to collect or share something new, this page will change first, and the
effective date above will move. Anything that changes where your data lives or who can see
it will also be announced in the app, with a link here, before it applies to you.

| Date | What changed |
|---|---|
| 2026-10-24 | First version. |
| 2026-10-25 | Described how invites work: a private iCloud link, and the name friends see. |
| 2026-11-03 | Said plainly that the limit on a friend's access (add a game, nothing more) is kept by the app, because iCloud gives invited friends write access. |
| 2026-11-05 | Brought the page up to date with the app: what is kept on your device (copies of friends' libraries, a sharing log, an undo history), the silent notifications from iCloud, that a friend's profile name is saved on a game they add, that Delete All My Data does not end sharing by itself, TestFlight's iCloud Diagnostics, and Support Info, a report you can read and send yourself with names and links removed. Nothing is sent by the app. |
| 2026-11-05 | Delete All My Data now also ends your sharing and deletes your profile name from iCloud (it no longer says it does not end sharing). |
| (date set when published) | Game details, covers and lists now come from IGDB through a small server run by the developer, which replaces "the developer has no server". Said what is sent to it and what is not, that two facts per game (main story time and game modes) are also kept in your private iCloud, and that IGDB's image servers see your IP address when pictures download. |

## Contact

Questions or requests: **naterowandev@gmail.com**
