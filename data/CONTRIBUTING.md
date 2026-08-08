# How to contribute data

Everything is optional. Even one item helps. You do not need a GitHub account and you do not need any technical skill.

## Where to send your answers

- **Easiest: email them to github.com/lzeo2/lenswatch/issues/new.** Plain words are fine. Write something like: "Kmart glasses, the LED lights up when recording and you can see it from the front, no pink glint". Attach any photos.
- Or open a GitHub issue: github.com/lzeo2/lenswatch/issues/new, tap "New issue", paste your answers, tap "Submit". A free GitHub account is needed, it takes about 2 minutes.
- Techy friend or teenager nearby? They can send it as a pull request. Not required.

If a question means nothing to you, skip it. A half filled in answer is still useful.

## The 4 measurements

### 1. Bluetooth scan (most valuable)
1. Install **nRF Connect** from the app store. It's free and it's the official app from Nordic, the company that makes the Bluetooth chips. Make sure it's "nRF Connect for Mobile" on Android, just "nRF Connect" on iPhone.
2. Open the **Scanner** tab. You'll see a list of every Bluetooth thing nearby (phones, headphones, cars). That's normal.
3. Turn your glasses on and open the app you set them up with (for Kmart glasses that app is called HeyCyan).
4. Your glasses will appear with a name like "Anko Smart Glasses". Look for it in the list and screenshot the whole screen.
5. The screenshot saves to your phone's Photos. You'll attach it to your email or issue.

Don't worry about the long numbers under each device. If you want to include one, copy the row that matches your glasses and take the first 6 characters (the part before the second colon). No need to understand what it means.

### 2. Lens glint photo
1. Point your phone's torch at the lenses from about 10-20cm away, at an angle.
2. Take a photo or video. A pink or purple dot or ring inside the lens means there's a camera sensor.
3. Do the same again while the glasses are recording, and compare.

### 3. Recording indicator
1. Start a recording (button or voice command).
2. Does an LED light up? Where? Can you see it from the front, the direction you'd be filmed from?
3. Can the LED be switched off in the settings, or covered with tape?

### 4. App and glasses
1. What's the app called that you set the glasses up with (HeyCyan, Meta AI, other)?
2. What brand and model are the glasses, where did you buy them, and how much were they?

## Format for techy people (optional)

If you know what you're doing, a PR with a JSON file is great. Or just copy this into an issue:

```json
{
  "brand": "Kmart Anko Smart Glasses",
  "price_aud": 89,
  "app": "HeyCyan",
  "ble_name": "",
  "ble_mac_prefix": "",
  "ble_services": "",
  "ir_glint": "yes/no/photo",
  "indicator_led": "front-visible/flashes/disableable/none",
  "shutter_sound": "yes/no",
  "notes": ""
}
```

Leave anything blank that you don't know.
