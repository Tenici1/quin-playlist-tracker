
## Tracking Twitch.tv/Quin69's Chat-Requested Songs
View this page at: https://tenici1.github.io/quin-playlist-tracker/

This is a fixed version after SheepFarmer stopped typing requested songs in chat. This version reads the full chat to fetch the channel redemptions. Since this is more data we also cache the result in local-storage to avoid fetching too much data.

Original:
https://github.com/orare/quin-playlist-tracker

**How It Works:**

We use Sheepfarmer's chat logs to see the current song, keeping the playlist up-to-date. Note that the accuracy depends on whether Quin69 uses the chat's playlist.

We read the full chat to fetch redemptions - since this is more data we also cache this and only fetch new messages each loop.

**Keeping It Accurate:**

If you spot a wrong song, it could be because:

- Quin69 isn't using the chat's playlist at that moment.
- The queue is out of date. To fix this, type `!song` in Quin69's chat to update the current song.
