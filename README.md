# Corner Crumb Bakery: Online Ordering Prototype

Room 2, Vibe Coding. A simple pickup-ordering tool for a fictional, pet-friendly neighborhood bakery. Open `index.html` in a browser; no install needed.

## Prompt log

| # | Prompt |
|---|--------|
| 1 | Build a simple online ordering tool for a neighborhood bakery. Customers should be able to browse baked goods, view prices, select quantities, choose a pickup date and time, and review their order before submitting it. Task: Generate a working prototype. Describe its main features and suggest three tests to check that it works correctly. |
| 2 | Pet-friendly atmosphere where pets and owners can enjoy a pastry. Hence, pet-friendly pastries are available for purchase. |
| 3 | Color theme of ivory/beige with pops of orange and blue similar to Secret Life of Pets movie color scheme. Customers should be able to select baked goods from a list but categorized into sweet goods and savory ones. |
| 4 | It should operate 24/7. |
| 5 | (Uploaded an image of a cartoon yellow Labrador with a blue collar and an orange ball; added as the bakery mascot.) |

## Main features

- **Sweet and savory lists:** 17 items in list form, grouped into Sweet (pastries, cookies and bars, whole cakes), Savory (breads, bagels and kolaches), and For pets, with filter buttons for All, Sweet, Savory, and For pets.
- **Color theme:** ivory and beige background with orange and blue accents; works in light and dark mode.
- **Mascot:** a yellow Labrador in the header (`images/mascot.jpg`).
- **Pet treats:** dog biscuits, a carrot pupcake, sweet potato chews, and a barkday cake (48 hours' notice), each labeled as made for dogs with no chocolate, xylitol, or raisins.
- **Pet check-in:** a "Bringing a pet?" box so the bakery can set out a water bowl; it shows on the review page.
- **Quantities:** plus and minus buttons or typed numbers; limit of 24 per item (3 per cake).
- **Baker's dozen pricing:** every 13th bagel is free.
- **Running order total:** updates as items change.
- **Pickup date and time:** open 24 hours, 7 days a week; dates from today to 14 days out; 30-minute slots around the clock (12:00 AM to 11:30 PM).
- **Notice rules:** orders need 2 hours' notice; whole cakes and the barkday cake need 48 hours, so earlier time slots disappear when a cake is in the order.
- **Contact info:** name and 10-digit phone required; optional notes for the baker.
- **Review before submitting:** a summary page with Edit order and Place order; placing the order gives an order number.

## Three tests

1. **Totals and baker's dozen.** Add 2 Butter croissants and 13 Plain bagels. Expected total: $8.50 + $21.00 = **$29.50**, with "1 free (baker's dozen)" under the bagels.
2. **Pickup rules.** Choose today: the first time listed should be at least 2 hours from now, and later dates should show slots all day and night, including overnight times like 2:00 AM. Then add an 8-inch carrot cake and choose tomorrow: no time slots earlier than 48 hours from now should appear.
3. **Review and submit.** Click Review order with an empty order and no contact info: error messages should list what is missing. Fill everything in, click Review order, check that the summary matches, click Edit order to confirm nothing was lost, then Place order and confirm an order number appears.

## Limits

This is a front-end prototype. Orders are not sent or saved anywhere; there is no payment, inventory, or bakery-side view.
