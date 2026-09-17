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
