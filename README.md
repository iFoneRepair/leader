# Office Closure Popup

`office-closure-popup.html` is a self-contained popup that announces the office
closure on **Thursday, Friday and Saturday, September 18–20, 2026**.

## How to add it to the homepage

1. Open the homepage template (for example `index.html`, or `theme.liquid` on Shopify).
2. Paste the full contents of `office-closure-popup.html` just before the closing `</body>` tag.
3. Save and publish.

## Behavior

- Appears immediately when the homepage loads.
- Can be dismissed with the **OK** button, the **×** button, the Escape key, or by clicking outside the box.
- Hides itself automatically after Saturday, September 20, 2026, so it does not need to be removed by hand.
- Works on phones and desktops (no dependencies, no external files).

## Changing the dates

Edit the text inside `<p class="closure-dates">` and the `closureEnds` date in the script.

---

# Booking Blackout Guard

`booking-blackout-guard.html` is a self-contained storefront snippet that stops
the appointment booking widget from offering slots on days the office is closed
(**September 18–20, 2026**), even when the app's own calendar blocks are ignored.

It is a safety net, not a replacement for fixing the block inside Appointment Pro.
Keep the app-side block in place as well.

## How to add it

1. Open the theme layout (`theme.liquid` on Shopify) or the page that hosts the booking widget.
2. Paste the full contents of `booking-blackout-guard.html` just before the closing `</body>` tag,
   **after** the booking widget's own script tag if it is also in the layout.
3. Save and publish.

## What it does

- Greys out and disables calendar day cells that fall on a blocked date, re-checking
  whenever the widget re-renders.
- Cancels clicks, taps and keyboard activation on a blocked date and shows a short
  "we are closed on that day" notice.
- Refuses add-to-cart requests and booking form submissions whose booking properties
  contain a blocked date, so a slot cannot slip through to checkout.
- Becomes inert automatically after Saturday, September 20, 2026.

## Changing the dates

Edit `BLOCKED_DATES` (YYYY-MM-DD, one per closure day) and `GUARD_ENDS` at the top of
the script. `NOTICE_TEXT` controls the message customers see.
