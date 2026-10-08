# Birthday-Wishes
# Birthday Surprise 🎂

A single-page, mobile-friendly birthday surprise for your girlfriend. She opens the link, types her name, blows out the candles, reads your message, and then plans her own party (date, time and place).

Everything lives in one file: `birthday.html` (HTML + CSS + JavaScript). No build step, no install, no backend.

## How it works

1. **Name** – the first screen asks only for the birthday girl's name.
2. **Cake** – the cake shows "Happy Birthday" with her name and the date `10/10/2026`. She taps the 3 flames to blow them out. Confetti pops and the floating balloons switch off.
3. **Lovely lines** – your message appears line by line and the screen scrolls along with it.
4. **Party plan** – she picks the date, the time (hour, minute, AM/PM) and the place (quick options or her own text).
5. **Thank you** – a summary of her choice, with buttons to send it to you on WhatsApp and to save it in Google Calendar.

## Features

- Floating balloons with different emojis, "Happy B'day" and her name, scattered randomly
- Confetti when the last candle goes out
- Handwriting-style text on the cake (Dancing Script)
- AM/PM time picker
- Light and dark theme (follows the phone setting)
- Mobile-first layout with big tap areas
- Respects "reduce motion" settings

## Run it

Open `birthday.html` in any modern browser. That is all.

Internet is only needed for the Google Fonts. Without it the page still works with default fonts.

## Put it online (get a link to send)

Pick any one:

- **Netlify Drop** – rename the file to `index.html`, go to `app.netlify.com/drop` and drag it in.
- **GitHub Pages** – upload `index.html` to a repo, then enable Pages in the repo settings.
- **Vercel** – import the repo or drag the folder in.

Send her the link on WhatsApp.

## Customise

Open `birthday.html` and search for these names:

| What to change | Where to look |
| --- | --- |
| Date on the cake | the line with `id="cd"` (default `10/10/2026`) |
| Your message to her | the `T` array inside the `lines()` function |
| Speed of the lines | `1700` (milliseconds per line) inside `lines()` |
| Place options | the `places` array |
| Default party time | `$('hh').value=7` and the `selected` option in `#ap` |
| Colours | `--rose` and `--gold` at the top, inside `:root` |
| Balloon emojis | the `wishEmojis` array |
| Number and colour of balloons | the `balloonColors` array (one balloon per colour) |
| WhatsApp message | inside the `thanks()` function |
| Page title | the `<title>` tag |

## Notes

- No data is stored or sent anywhere. Her name and choices stay in her browser.
- The WhatsApp and Calendar buttons open WhatsApp and Google Calendar in a new tab with the details already filled in. She picks who to send to.
- Calendar events are set to last 3 hours.
- Tested for script errors only in a simple automated check. Please open it on a real phone once before you send the link.

## Tech

Plain HTML, CSS and JavaScript. Fonts: Caprasimo, Dancing Script and DM Sans from Google Fonts.

Made with love. ❤️
