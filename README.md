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

# Mobile Product Title Layout

`product-title-mobile.html` fixes the product page on phones: the title no
longer sits squeezed and centered in the column next to the product image.
Instead it spans the full width at the top of the product section and is
left aligned. Desktop layout is unchanged.

## How to add it

1. Open the theme layout (`theme.liquid` on Shopify).
2. Paste the full contents of `product-title-mobile.html` just before the closing `</body>` tag.
3. Save and publish.

## Behavior

- Runs only on screens 749px wide or narrower (phones).
- Finds the product title (the `h1` nearest the add-to-cart form) and moves it
  above the image gallery, full width and left aligned.
- Moves the title back to its original spot if the window grows past 749px.
- Works with any theme; no dependencies.

## Adjusting

- Change the `749px` value in both the `<style>` and `<script>` blocks to use a
  different breakpoint.
- Change `font-size: 24px` in the `<style>` block to resize the mobile title.
