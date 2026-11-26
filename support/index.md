---
layout: default
title: "Pixel In Waiting — Support"
---

# Pixel In Waiting — Support

Pixel In Waiting is made by one person, Nate Rowan. If something is not working or you have
a question, email **naterowandev@gmail.com**. I read every message.

## Getting help with a problem

The app can write a short report that helps me see what went wrong:

1. Open **Settings ▸ Support Info** (on iPhone and iPad: the gear on Home).
2. Read the report. It holds the app and system versions, the iCloud status, counts and a log
   of sharing events with their times. Names are replaced with "Me" and "Friend 1", "Friend 2",
   and links, email addresses and long IDs are removed or cut short.
3. Tap **Copy** or **Share** and send it to the address above, with a line about what you were
   doing.

Nothing is sent unless you send it.

## Common questions

**My games are not syncing between my Mac, iPhone and iPad.**
Check that both devices are signed in to the same iCloud account and that iCloud is on for
Pixel In Waiting (Settings ▸ iCloud on iPhone or iPad, System Settings ▸ Apple Account ▸ iCloud on
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
Open the game and look at **You own it on** in the Your Game card. Choose **Add a platform**, then set how you
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

**Can the app fill in the platform for me?**
Yes. In **Settings**, choose a **Default platform**. When you mark a game Owned, Playing, Played or Abandoned and its
platform is empty, the app fills in the default, if the game is on that platform. It never replaces a platform you
set, and the setting is kept on this device only.

**Can I change the status, interest or platform of many games at once?**
On iPhone or iPad, tap **More ▸ Select Games** (or press and hold a game and choose **Select**), tick the games, then tap
**Change**. On Mac, select the games and right-click. You can set their status, interest level and platform. Games
that already have a platform, or are not on the one you pick, are left alone, and the app tells you which. **Recent
Changes** can undo it for three days.

**Can I change what Home shows?**
Yes. Tap the slider icon at the top of Home, beside your profile picture (also in **Settings ▸ Customize Home…**).
Drag the tiles to reorder them, switch one off to hide it, or choose **Reset** to go back. The layout is saved on that
device only.

**Can I change what Play Next shows?**
Yes, the same way: tap the slider icon at the top of Play Next (also in **Settings ▸ Customize Play Next…**). Every
section can be moved or hidden, including **Who's playing** and the list of games. The layout is saved on that device
only.

**What are the Best Picks on Play Next?**
Up to five cards, each a different game: **Best pick** (what people want most), **Critics' choice**, **New and
wanted**, **Recently bought** (the Owned game you added most recently, have not started and rate 7 or higher; the
date is when you added it) and **Best wishlist pick**. A game on your Wishlist appears only in the last one: a sale
of 30% or more on a game you rate 7 or higher or the critics score 80 or higher, otherwise the highest critic score.
A card is left out when no game fits.

**Why is a game missing from Play Next?**
Play Next shows every game that someone you picked could play now: Playing, Ongoing, Owned or Wishlist. An interest
level is not needed, and games with one come first. A game that is not out yet, or comes out more than two weeks from
now, is in **Coming Soon** instead (soonest first; a game with no date is last). A game is left out when you have
played or abandoned it, or when everyone who could play it has marked it **Not Interested**. If you hid a section in
**Customize Play Next**, its games are not shown.

**How do I tell the app I am not interested in a game?**
On the game's page, tap the **⊘** before the ten flames in **My Interest** (tap it again to clear it). You can also
press and hold a game on iPhone or iPad, or right-click it on Mac, and choose **Interest Level ▸ Not Interested**,
including on Play Next. It sets the interest to 0: the game leaves your Play Next unless a friend still wants it, and
then your circle shows a cancel sign. Friends you share with see it like the rest of your library. A version older
than 3.1.0 skips a game marked this way until it is updated.

**What is Ongoing?**
A status for a game you keep playing and never finish, like an online or endless game. Choose it from the game's
**Status**. It has a start day and no end day, stays in **Not Played** and **Play Next** so you are offered it again,
shows in Playing now, and does not count in your played numbers. Mark it Played or Abandoned whenever you are done. A
version older than 3.1.0 skips an Ongoing game until it is updated.

**A banner says some games can't be read by this version of the app.**
Tap the banner to see which games and why. Most often your iCloud library holds games that a newer version of the app
added, for example one marked Ongoing or Not Interested, and updating the app on this device shows them. If the reason
says the data is missing or damaged, an update won't change it: send Settings ▸ Support Info, which lists the same
reasons, to the developer. Nothing is lost.

**How do I search for a game?**
Open **Add a Game** and start typing a title. When you pause, and have typed at least three letters, the app searches by
itself and shows the results. For a shorter title, press Return or tap the **Search** button that appears. The lists
under the search box (popular, new, coming soon) are there until you search.

**How does price tracking work?**
**Settings ▸ Price tracking ▸ Track prices.** It is on by default. The app looks up the PlayStation Store price, in US
dollars, of the games on your Wishlist through the developer's server, which is sent only those games' IGDB names.
Prices show under titles, on Home's Wishlist deals tile and in a Pricing section on the game's page. Pick PS5 or PS4
as the platform. Turn the switch off to stop lookups. Your copy of the prices stays on your device, and **Delete All My
Data** removes it.

**A friend sent me their list as a CSV or JSON file. How do I open it?**
On iPhone or iPad, tap the file in Messages or Files, then choose share and **Pixel In Waiting**. On Mac,
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
**Settings ▸ Release reminders ▸ Remind me on release day.** Turning it on asks your Mac, iPhone or iPad for permission to show notifications. If you said no, allow Pixel In Waiting in System Settings ▸ Notifications and try again. You get one notification at 9 AM on the day a game on your Upcoming list comes out, and only for games with an exact date. Tap it to open the game. Turning the switch off removes them.

**The sync line says "Another device just changed a game. Syncing again…"**
Two of your devices changed the same game at about the same time. The app syncs again by itself; nothing is lost. If it stays on that line, open the app on the other device and try **Sync Now** in **Settings ▸ iCloud**.

**Where does my data live?**
Your library is on your device and in your own iCloud account. Game details and covers from IGDB are
looked up through a small server and saved only on your device, apart from a few facts per game (its three times to beat
and game modes) that also sit in your private iCloud. Unless you turn off **Price tracking** in Settings (it is on by default), the
names of the games on your Wishlist are also sent to that server to look up PlayStation Store prices. The server keeps
each game's prices, never who asked or which games you have, and your copy of the prices stays on your device. See the
[Privacy Policy](../privacy/).

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
