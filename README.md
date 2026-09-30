# Duology (prototype) + Duology Studio

**Duology:** astrology and numerology, explained. Your birth chart in plain English, with the *why* behind every placement. It also covers forecasts, numerology and general star-sign readings.

**Duology Studio:** the companion tool that turns each month's star-sign readings into a 5 to 7 minute YouTube forecast. It gives you the script, recordable video scenes, Shorts and the YouTube description.

Both are single HTML files with no build tools and no dependencies.

## Deploy to GitHub Pages

1. In the **SCVD-App** org, create a new repo called `duology` (public).
2. Click **Add file → Upload files**, drag in `index.html`, `studio.html` and this `README.md`, then **Commit changes**.
3. Go to **Settings → Pages**. Set **Source: Deploy from a branch**, **Branch: main**, folder **/ (root)**, then **Save**.
4. After a minute or two:
   - The app is at `https://scvd-app.github.io/duology/`
   - The Studio is at `https://scvd-app.github.io/duology/studio.html`. It's set to *noindex*, so search engines won't list it, but anyone with the link can open it. Don't put the link anywhere public.

To update, upload the new file(s) over the old ones and commit.

## Deep links for YouTube

Link viewers straight to their sign's month:

`https://scvd-app.github.io/duology/#sign=leo` (use any sign name: aries, taurus, gemini, and so on)

No birth details are needed. Viewers see the general reading for their sign, and a button invites them to build their personal chart.

## What's in Duology

- **Personal chart:** a labelled wheel, the Big Three, every placement, element mix and aspects. Every card has What it means, Why they say that, the house, How it fits the rest of your chart, and Keep in mind.
- **My forecast:** real transits for 30 days, 90 days and 12 months. Each event says where it lands in your chart, how long it lasts, how much it counts and which retrograde pass it is. Also includes sign changes, stations, New and Full Moons, eclipses, your solar return, and Personal Year and Month changes.
- **Star signs:** a monthly reading for each of the 12 signs, worked out with solar houses. Includes:
  - The month's theme house
  - Recharge days
  - The Universal Month number
  - The big events for that sign, then everything else, with + drill-downs on each
  - "The sky this month, explained"
  - A birthday sign finder, with a note if you were born on the cusp
- **Numbers:** Life Path, Expression, Soul Urge, Personality, and Personal Year and Month, with how they play off each other. Every number shows its working.
- **Learn:** 13 short lessons.
- **Settings:** saved charts, house system, numerology system, master numbers and delete-all.

## Making the monthly video with Duology Studio

1. **Pick the month.** Studio jumps to next month automatically after the 15th.
2. **Script tab.**
   - Choose a depth: Tight (about 6 min), Standard (about 7 min) or Deep (10+ min).
   - Set the voice pace to match your AI voice. Most sit around 150 to 170 words a minute.
   - Edit anything you like. Edits are saved in your browser and marked "edited".
   - **Copy voice script** gives you clean text to paste into your AI voice tool.
   - **Download script** gives you the same text with scene markers and timings.
3. **Video tab.**
   - Start your screen recorder: OBS, or Windows Game Bar (Win + Alt + R).
   - Press **H** for clean mode or **F** for full screen, then **Space** to play.
   - Each scene holds for as long as its voiceover runs. The arrow keys step through scenes, and Esc exits clean mode.
4. **Put it together** in your editor: drop the AI voice track over the recording and nudge the timing to match.
5. **YouTube tab.** You get three title ideas and a ready description with chapter timestamps, the app link, the "for reflection" line and the AI-narration disclosure. Adjust the chapter times once you have the real voice track.
6. **Shorts tab.** There's a 9:16 version for each sign, about 45 to 55 seconds. Record each one the same way, or use **Download all 12 Shorts scripts**.

## Accuracy

The calculations were checked against the Swiss Ephemeris:

- **Sun, Moon, Mercury, Venus, Mars, Uranus, Neptune and Pluto:** within 0.03°.
- **Jupiter and Saturn:** within 0.16°.
- **Rising sign, Midheaven and Placidus house cusps:** within 0.01°.
- **Eclipses:** the eclipse detection matched every real eclipse from 2024 to 2026.

The calculations are designed for 1800 to 2050.

Dates in both apps use the timezone of the device they're opened on. Studio says which timezone it's using in the script.

## Before the channel goes live

- **Paywall:** add a Pro unlock (full personal chart and forecast) through a Stripe Worker. Keep the star-sign readings free, since they're the funnel from the channel.
- **Make each video its own:** give every month's script a personal pass before recording. YouTube's rules against mass-produced, repetitive content can cost you monetisation, and your own edits are the best protection.
- **Privacy note:** add one to the app.
