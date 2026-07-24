# Rumble Run Club — Full Campaign Playbook

---

# ⚠️ PRE-FLIGHT — DO THIS BEFORE SCHEDULING ANYTHING

## Step 1. Upload 8 new images to the repo

Upload these into `OliD12345678/rumble-run-club-email/assets/`. They are numbered to
continue your existing 01-06 scheme, so nothing overwrites and nothing collides.

| File | Used by |
|---|---|
| `07-week-out.jpg` | Email 2 |
| `08-tomorrow-aug8.jpg` | Email 3 |
| `09-morning-aug8.jpg` | Email 4 |
| `10-encore-aug15.jpg` | Email 5 |
| `11-tomorrow-aug15.jpg` | Email 6 |
| `12-morning-aug15.jpg` | Email 7 |
| `13-thank-you.jpg` | Email 8 / 8a |
| `14-missed-it.jpg` | Email 8b |

Your existing `01-hero.jpg` through `06-see-ya-then.jpg` stay exactly as they are.
The campaign emails now reference them by their real names and reuse them.

## Step 2. Verify one image is live

Open this in a browser. If it loads, GitHub Pages has published and every other
image will work too. If it 404s, wait 2 minutes and refresh — Pages can lag.

```
https://olid12345678.github.io/rumble-run-club-email/assets/07-week-out.jpg
```

**Do not schedule anything until this loads.** This is the single most common way
an email campaign ships broken.

## Step 3. Send yourself a test

Paste `02-week-out.html` into ClubReady's HTML/source view, send to yourself only,
then open it on your phone in Gmail. Check:

- [ ] All 4 images load (hero, Aug 8 card, Do The Double, PLN banner)
- [ ] Hero and button both link to the signup page
- [ ] Signup form still submits and the studio inbox receives it
- [ ] ClubReady's unsubscribe + address footer is present

Only after that passes do you schedule the real send.

---

## Ready-to-send status

| Email | Blocking issue | Ready? |
|---|---|---|
| 2 — Week out | Needs `07-week-out.jpg` uploaded | ✅ after Step 1 |
| 3 — 24hr Aug 8 | Needs `08-tomorrow-aug8.jpg` | ✅ after Step 1 |
| 4 — Morning Aug 8 | Needs `09-morning-aug8.jpg` | ✅ after Step 1 |
| 5 — Encore | Needs `10-encore-aug15.jpg` | ✅ after Step 1 |
| 6 — 24hr Aug 15 | Needs `11-tomorrow-aug15.jpg` | ✅ after Step 1 |
| 7 — Morning Aug 15 | Needs `12-morning-aug15.jpg` | ✅ after Step 1 |
| 8a — Attendees | Needs `13-thank-you.jpg` **+ your offer + booking URL** | ⛔ offer required |
| 8b — Non-attendees | Needs `14-missed-it.jpg` **+ your offer + booking URL** | ⛔ offer required |

Emails 2 through 7 are fully written and need nothing from you but the image upload.
Emails 8a and 8b cannot send until you write the offer — they contain literal
`[YOUR OFFER HERE]` and `https://YOUR-BOOKING-LINK` placeholder text.

## One visual check

Your live `02-aug8-lindsay.jpg` may or may not be the mirror-flipped version of
Lindsay's photo — the flip was the last thing generated before the session ended,
so the file you deployed may predate it. Open the live URL and confirm her face is
on the left and clear of the text. If it isn't, that's a 30-second regenerate, not
a blocker for Email 2.

---

## Campaign at a glance

| # | Send | Day/Time | From | Subject A | Subject B | File |
|---|------|----------|------|-----------|-----------|------|
| 1 | ✅ shipped | Jul 23 | Rumble Alpharetta | (your original) | — | (already sent) |
| 2 | **Aug 1** | Fri 7:00 AM | Rumble Alpharetta | One week out. You in for Saturday? | This time next week: Rumble Run Club | `02-week-out.html` |
| 3 | **Aug 7** | Fri 4:00 PM | Coach Lindsay | Tomorrow. 8:30 AM. Bring water. | See you tomorrow at Run Club? | `03-tomorrow-aug8.html` |
| 4 | **Aug 8** | Sat 6:00 AM | Rumble Alpharetta | ☀️ This is your alarm. 8:30 AM. | 8:30 AM. Shoes on. | `04-morning-aug8.html` |
| 5 | **Aug 9** | Sun 10:00 AM | Rumble Alpharetta | Round two. Aug 15. | That was something. One more shot. | `05-encore-aug15.html` |
| 6 | **Aug 14** | Fri 4:00 PM | Coach JP | Last chance. Tomorrow. 8:30. | Round two goes tomorrow. | `06-tomorrow-aug15.html` |
| 7 | **Aug 15** | Sat 6:00 AM | Rumble Alpharetta | ☀️ Last round. 8:30 AM. | Coach JP is warming up. | `07-morning-aug15.html` |
| 8a | **Aug 17** | Mon 10:00 AM | Drew Oliver | You showed up. Now what? | Two Saturdays. Now let’s talk. | `08a-thank-you-attendees.html` |
| 8b | **Aug 18** | Tue 10:00 AM | Drew Oliver | You missed this one. | The next one is yours. | `08b-thank-you-nonattendees.html` |

**A/B advice:** run A on the first 5,000, B on the next 5,000, then use the winner for the second event. Track opens and RSVPs by subject in ClubReady reports.

**From-name strategy:** the two 24-hour reminders come from the individual coach leading that Saturday. Personal from-names lift opens 15-25% on transactional-feeling reminders. The morning-of and thank-you shifts back to the studio / owner voice.

## Deployment steps

### 1. Add the 7 new hero images to your GitHub repo
Upload everything in `assets/` to `OliD12345678/rumble-run-club-email` under the `/assets/` folder. Your existing 6 images stay, these 7 new heroes join them:

- `02-week-out-hero.jpg`
- `03-tomorrow-aug8-hero.jpg`
- `04-morning-aug8-hero.jpg`
- `05-encore-hero.jpg`
- `06-tomorrow-aug15-hero.jpg`
- `07-morning-aug15-hero.jpg`
- `08-thank-you-hero.jpg`

Verify one image loads at `https://olid12345678.github.io/rumble-run-club-email/assets/02-week-out-hero.jpg` before scheduling anything.

### 2. Fill in the conversion offer on Email 8
Email 8 has a clearly marked placeholder for `[YOUR OFFER HERE]` and `https://YOUR-BOOKING-LINK`. Three offer patterns that convert well for event-warmed prospects:

- **First class free + intro membership rate.** Lowest friction. "Come back this week, first class is on us."
- **Founding member lock-in.** Scarcity-driven. "First 20 RSVPs get [$X/mo for life]. Expires Aug 24."
- **Community continuation.** Longer arc. "Run Club becomes monthly. Membership includes automatic entry."

Pick one, write it in your own voice, replace the button URL with the correct ClubReady booking or Connect landing link.

### 3. Send flow in ClubReady
Same pattern you used for Email 1:
1. Open ClubReady email composer, switch to HTML/source view.
2. Paste the file contents.
3. Send test to yourself. Open in Gmail mobile specifically.
4. Send to your prospect + member segments.

Keep ClubReady's unsubscribe footer and physical address enabled on every send — required for CAN-SPAM.

## Segmentation notes

Ideally the reminder emails (3, 6, 7) go only to people who RSVP'd for that specific event, but if the FormSubmit relay doesn't feed back into ClubReady segments cleanly, sending to your full 12k list is fine. The energy is community-forward, non-RSVPs won't feel excluded.

Email 8 is the money email — highest intent segment. If ClubReady tracks event attendance (or you can flag attendees manually), send Email 8's offer at a different tier to attendees vs non-attendees. Attendees convert 3-5x higher.

## What to measure

- **Opens per email.** Anything under 25% for an engaged fitness list means your subject line needs work.
- **Clicks to signup page.** Anything under 3% of opens means the CTA isn't compelling enough.
- **RSVPs per email.** Watch which reminder drives the most late RSVPs — that tells you when your list actually reads email.
- **Attendance rate.** RSVPs vs door count. Under 60% means your reminders aren't landing or your ask is too casual.
- **Conversion rate on Email 8.** Under 5% of attendees converting means your offer needs sharpening.

Give me the numbers after each send and we can adjust the next one before it goes out.


---

## Segmented close (Emails 8a / 8b)

`08-thank-you.html` is the generic version, kept as a fallback if you can't segment. Prefer these two:

- **`08a-thank-you-attendees.html`** — people who actually showed. Hottest segment in the campaign. Strongest offer goes here, with a deadline. Send Mon Aug 17.
- **`08b-thank-you-nonattendees.html`** — RSVP'd or opened but never came. Zero guilt, lower-friction offer, standing invitation. Send Tue Aug 18, one day later so the two don't collide in a shared inbox.

Both have the same `[YOUR OFFER HERE]` and `https://YOUR-BOOKING-LINK` placeholders. Write the attendee offer first, then soften it for 8b.

**Capturing attendance:** the cheapest version is a clipboard at the door and 10 minutes of data entry Saturday afternoon. Do not skip it. The difference between a segmented and unsegmented close is usually the difference between a 3% and a 12% conversion rate on this kind of event.

## SMS layer

See `SMS-SCRIPTS.md` for 10 companion texts mapped to the same calendar, each pre-counted for single-segment sending. Texts go to RSVPs and members only, never the cold 12k. The highest-value one is the same-day thank you on Aug 8 at noon, it books the second Saturday while people still feel great.
