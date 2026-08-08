# LensWatch

Know when someone might be recording you.

Camera smart glasses went mass market in Australia. Kmart sold $89 pairs that sold out in a week, and there's no enforced recording indicator. You can't tell if the person next to you is filming you. That's a problem for everyone, but it's worst for women, for kids, and for parents who can't see what a stranger's glasses are doing near their child.

## Where we're up to (honest)

LensWatch is **not finished yet. There is no app to download today.** We are building it, and the fastest way to make it real is the 2-minute tasks below.

When it's done, it will be two parts:
1. A **free phone app** that warns you when it spots a camera signal nearby.
2. An optional small detector gadget (matchbox-sized, about $20 of parts) that the app talks to.

You do **not** need to buy or build anything to help today.

## Do I need to buy anything?

To use the finished app you'll need an **Android phone** (an iPhone version is planned, not ready). The app will be **free**. The optional gadget is about **$20 of parts**, and we'll post simple build instructions when it's ready. To help today, you need nothing except the glasses you own and your phone.

## Who this is for

Anyone who doesn't want to be secretly recorded. We're building it with women and parents of young kids in mind first, because they're the ones carrying the risk day to day. Feedback from those communities is the most valuable there is.

## How it finds hidden cameras (plain English)

- **Lenses glint.** Like a cat's eyes at night, a camera lens shines when light bounces off it. A quick flash from our detector makes a hidden lens glow pink or purple for a split second.
- **Smart glasses announce themselves.** Glasses talk to your phone by Bluetooth, and when they do they send a name and a number. We're building a list of the names and numbers that camera glasses use, so the app can recognise them.
- **Phones chat to WiFi.** Phones and glasses send out little "are you there?" pings. The app can listen for those too.

You don't need to understand any of this to help. The tasks below tell you exactly what to do. (And "ESP32" is just the name of the chip inside the optional gadget. You can ignore it.)

## Send us your answers (pick whichever is easiest)

- **Easiest: email them to github.com/lzeo2/lenswatch/issues/new.** Plain words are fine, no special format, photos welcome.
- Or open a "GitHub issue": go to github.com/lzeo2/lenswatch/issues/new, tap "New issue", paste your answers, tap "Submit". You'll need a free GitHub account first (takes 2 minutes). A GitHub issue is just a public message board post, nothing scary.
- Or, if a techy friend or your teenager is around, they can send it as a pull request. Not required.

If the form below looks confusing, ignore it and just write: **the brand of glasses, what you saw, and your photo.** Blank boxes are fine, we can still use it.

| # | Task | How | Time |
|---|---|---|---|
| 1 | Bluetooth scan | Install nRF Connect (free, from the chip company Nordic), open Scanner, turn your glasses on, screenshot the device list | 2 min |
| 2 | Lens glint photo | Shine your phone torch at the lenses at an angle, photo the reflection (a pink/purple glint means camera sensor) | 1 min |
| 3 | Indicator check | Start recording. Does an LED light up? Visible from the front? Can it be disabled? | 1 min |
| 4 | App name | Which app did you set the glasses up with? (for Kmart glasses it's called HeyCyan) | 10 sec |

Full step by step instructions: see data/CONTRIBUTING.md

No glasses? You can still help. Send ideas to the email above, or comment on an issue.

## Who's behind this? Is it safe?

LensWatch is a community project started by a Canberra teenager. It's **open source**, which means the instructions are public for anyone to check. You don't have to take our word for it, independent people can verify it does what it says.

Your photos and screenshots are used only to build the detection list. We won't share your name or details, and you can ask us to delete anything you send. If anything feels off, open a GitHub issue (free account, 2 minutes): github.com/lzeo2/lenswatch/issues/new, a real person reads it.

## The build (planned)

- Tier 1: phone-only Android app. Bluetooth/WiFi unknown device scanner and a lens reflection test
- Tier 2: ESP32 sniffer (WiFi and BLE scanning) streaming to the phone app
- Tier 3: RF detector module and IR flash

## Honest limits

This can't detect every camera, defeat determined stalkers, or do wideband RF sweeps without extra hardware. It's a practical tool, not a guarantee. If you're in immediate danger, contact the authorities.
