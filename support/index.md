---
layout: default
title: "Pixel In Waiting — Support"
---

# Pixel In Waiting — Support

Pixel In Waiting is made by one person, Nate Rowan. If something is not working or you have
a question, email **naterowandev@gmail.com**. I read every message.

## Getting help with a problem

The app can write a short report that helps me see what went wrong:

1. Open **Settings ▸ Support Info** (on iPhone: the gear on Home).
2. Read the report. It holds the app and system versions, the iCloud status, counts and a log
   of sharing events with their times. Names are replaced with "Me" and "Friend 1", "Friend 2",
   and links, email addresses and long IDs are removed or cut short.
3. Tap **Copy** or **Share** and send it to the address above, with a line about what you were
   doing.

Nothing is sent unless you send it.

## Common questions

**My games are not syncing between my Mac and iPhone.**
Check that both devices are signed in to the same iCloud account and that iCloud is on for
Pixel In Waiting (Settings ▸ iCloud on iPhone, System Settings ▸ Apple Account ▸ iCloud on
Mac). Sync needs a connection; the app works offline and catches up later.

**A friend's invite does not work.**
The link only works for the person it was sent to, and only while they are signed in to iCloud
with the account that was invited. If it does not open, send a new invite from **Friends**.

**How do I stop sharing with someone?**
In **Friends**, use **Stop Sharing** for that person (or **Cancel Invite** if they have not accepted yet). They stop seeing your library. You can also
remove them from your list.

**How do I get my games out of the app?**
**Settings ▸ Export** saves your library as CSV or JSON. You can import a file the same way. The JSON export
can include **Platforms Owned On**, and restoring that file brings the platforms back.

**Which platform did I play a game on? Can I own it on more than one?**
Open the game and look at **Platforms you own it on** in the Your Game card. **Add** a platform, then set how you
have it (purchased or subscription), its started and ended days and its hours. Each platform keeps its own days and
hours, and the game keeps one status. The platform marked **Platform Played** is the one the game's own Started and
Ended days follow. Friends you share with can see these platforms.

**A game was added as the wrong edition (for example the PC release of a game I played on PlayStation). How do I fix it?**
Open the game and click the small **Wikidata** tag above the Your Game card. Search for the right game and pick it.
Everything you entered (status, rating, notes, platforms, days and hours) moves to that game. If you already have the
other game, the two are merged and you are asked first. **Recent Changes** can undo it for three days.

**Can I import play time and dates from a file?**
Yes. The **advanced import** reads a JSON file in a documented format (see [the file](#the-advanced-import-file-version-1)
below) and fills in platforms, hours and dates for games it finds by their Wikidata ID. Choose **Settings ▸ Import**,
or open the file from Messages or Files. Nothing changes until you have looked over the review, where games are
grouped (New Games, Updates, Probably Finished, Not Found, No Change). It adds missing games and fills blanks, and a day
that conflicts with one you already have is offered unticked, so yours stays unless you tick it. The file is read on your device and is never sent anywhere. One
**Undo Import** (or **Recent Changes**, for three days) reverses the whole import. Importing the same file again
changes nothing.

**A friend sent me their list as a CSV or JSON file. How do I open it?**
On iPhone, tap the file in Messages or Files, then choose share and **Pixel In Waiting**. On Mac,
right-click the file in Finder and choose **Open With ▸ Pixel In Waiting**. The app opens the same
import screen as in Settings, so you can see what will be added first; **Cancel** adds nothing.
A list from another copy of the app starts on **Restore missing only**, so games you already have are
kept as they are, and **Recent Changes** can undo an import for three days.

**How do I delete my data?**
**Settings ▸ Delete All My Data** (on Mac also File ▸ Delete All My Data). It removes your
library, history, friends and settings from your device and from iCloud, ends your sharing and
deletes your profile name. It cannot be undone, so export first if you want a copy.

**I removed a game by mistake.**
**Recent Changes** keeps removals and imports for three days, and you can undo them there.

**Covers, time to beat or ratings are missing for a game.**
The details come from IGDB, which does not know every game. Check you are online, then open the game
again; the app asks again when its saved details are a week old for a new game, or three months for an
older one. **Settings ▸ Game data ▸ Refresh Game Data** asks again now, once an hour. If the data service
is very busy, the app shows placeholders and fills them in later.

**How do I clear the covers and details the app saved?**
**Settings ▸ Game data ▸ Clear Cached Game Data.** They are saved only on your device and come back when
you open a game. Your library is not touched.

**How do I turn release-day reminders on or off?**
**Settings ▸ Release reminders ▸ Remind me on release day.** Turning it on asks your Mac or iPhone for permission to show notifications. If you said no, allow Pixel In Waiting in System Settings ▸ Notifications and try again. You get one notification at 9 AM on the day a game on your Upcoming list comes out, and only for games with an exact date. Tap it to open the game. Turning the switch off removes them.

**The sync line says "Another device just changed a game. Syncing again…"**
Two of your devices changed the same game at about the same time. The app syncs again by itself; nothing is lost. If it stays on that line, open the app on the other device and try **Sync Now** in **Settings ▸ iCloud**.

**Where does my data live?**
Your library is on your device and in your own iCloud account. Game details and covers from IGDB are
looked up through a small server and saved only on your device, apart from a few facts per game (its three times to beat
and game modes) that also sit in your private iCloud. See the [Privacy Policy](../privacy/).

## The advanced import file (version 1)

Anyone who can make a JSON file in this shape can import it with the advanced import. The app reads only the keys below
and ignores everything else. A key that is left out means "unknown" and changes nothing; a blank is never written over
something you have. **Version 1 is a promise:** the app will keep reading it. Any key added later is optional, and a file
marked with a newer `formatVersion` than the app knows is refused with a message, not half read.

```json
{
  "format": "store-importer",
  "formatVersion": 1,
  "sources": [{ "store": "playstation", "complete": true }],
  "games": [
    {
      "title": "Made Up Game",
      "wikidataID": "Q000000",
      "storeRecords": [
        {
          "owned": true,
          "ownedBasis": "purchased",
          "platformPlayed": "PS5",
          "hours": 21.5,
          "firstPlayed": "2024-01-02T10:00:00Z",
          "lastPlayed": "2024-03-04T20:00:00Z",
          "achievements": { "platinumEarnedOn": "2024-03-01" }
        }
      ]
    }
  ]
}
```

_The game, ID and figures are made up._

| Key | What the app does with it |
|---|---|
| `format`, `formatVersion` | `format` must be `store-importer`; `formatVersion` is `1`. A newer version is refused |
| `sources[].store`, `sources[].complete` | Named on the review screen. A partial file (`complete: false`) is still safe: the import only adds and fills |
| `games[].wikidataID` | **Required.** The game is found by this ID. A game with none, or listed twice, is left out and counted |
| `games[].title` | Shown in the review, and for an ID that can't be found |
| `storeRecords[]` | One entry per copy of the game on a platform |
| `owned`, `wishlisted` | Owned, or on a wishlist (a wishlist-only game is added as Wishlist or Upcoming) |
| `ownedBasis` | `purchased`, `subscription` or `play_history` |
| `platformPlayed`, `platforms` | The platform of the copy (the first of `platforms` if `platformPlayed` is missing). Known names such as `PS5`, `PS4`, `Microsoft Windows`, `macOS`, `Xbox One`, `Xbox Series X/S` |
| `hours` | Hours played on that platform (left out at 0) |
| `firstPlayed`, `lastPlayed` | A UTC time or a day. Fills Started and Last played |
| `achievements.platinumEarnedOn`, `completedOn` | A day the game was finished; used as the Ended day |
| `achievements.storyBand` (`earned`, `total`, `lastEarnedAt`) | When 85% or more of the story achievements are earned, the game counts as finished |
| `achievements.items[].earnedAt` | The earliest day stands in for a missing first played |

The achievements themselves are not kept, only these dates. The file holds no name, email, account or token, and the
app does not read any.

[Back to Pixel In Waiting](../)
