# Corner Crumb Bakery: Online Ordering Prototype

Room 2, Vibe Coding. A simple pickup-ordering tool for a fictional neighborhood bakery. Open `index.html` in a browser; no install needed.

## Prompt log

| # | Prompt |
|---|--------|
| 1 | Build a simple online ordering tool for a neighborhood bakery. Customers should be able to browse baked goods, view prices, select quantities, choose a pickup date and time, and review their order before submitting it. Task: Generate a working prototype. Describe its main features and suggest three tests to check that it works correctly. |

## Main features

- **Menu with prices:** 13 items in five categories (breads, pastries, bagels, cookies and bars, whole cakes), with a filter by category.
- **Quantities:** plus and minus buttons or typed numbers; limit of 24 per item (3 per cake).
- **Baker's dozen pricing:** every 13th bagel is free.
- **Running order total:** updates as items change.
- **Pickup date and time:** dates from today to 14 days out; 30-minute slots from 7:00 AM to 1:30 PM; closed Mondays.
- **Notice rules:** orders need 2 hours' notice; whole cakes need 48 hours, so earlier time slots disappear when a cake is in the order.
- **Contact info:** name and 10-digit phone required; optional notes for the baker.
- **Review before submitting:** a summary page with Edit order and Place order; placing the order gives an order number.

## Three tests

1. **Totals and baker's dozen.** Add 2 Butter croissants and 13 Plain bagels. Expected total: $8.50 + $21.00 = **$29.50**, with "1 free (baker's dozen)" under the bagels.
2. **Pickup rules.** Choose a Monday: the time list should say "Closed Mondays." Then add an 8-inch carrot cake and choose tomorrow: no time slots earlier than 48 hours from now should appear.
3. **Review and submit.** Click Review order with an empty order and no contact info: error messages should list what is missing. Fill everything in, click Review order, check that the summary matches, click Edit order to confirm nothing was lost, then Place order and confirm an order number appears.

## Limits

This is a front-end prototype. Orders are not sent or saved anywhere; there is no payment, inventory, or bakery-side view.
