# Corner Crumb Bakery: Online Ordering Prototype

Room 2, Vibe Coding. A simple ordering tool for a fictional, pet-friendly bakery that delivers anywhere in the world, 24/7. Open `index.html` in a browser; no install needed.

## Prompt log

| # | Prompt |
|---|--------|
| 1 | Build a simple online ordering tool for a neighborhood bakery. Customers should be able to browse baked goods, view prices, select quantities, choose a pickup date and time, and review their order before submitting it. Task: Generate a working prototype. Describe its main features and suggest three tests to check that it works correctly. |
| 2 | Pet-friendly atmosphere where pets and owners can enjoy a pastry. Hence, pet-friendly pastries are available for purchase. |
| 3 | Color theme of ivory/beige with pops of orange and blue similar to Secret Life of Pets movie color scheme. Customers should be able to select baked goods from a list but categorized into sweet goods and savory ones. |
| 4 | It should operate 24/7. |
| 5 | (Uploaded an image of a cartoon yellow Labrador with a blue collar and an orange ball; added as the bakery mascot.) |
| 6 | (Uploaded three more images: an orange tabby cat, a gray and white cat, and a terrier puppy.) Add images to site. |
| 7 | (Uploaded the Corner Crumb Bakery logo.) Push. |
| 8 | When pets is selected the heading is to the left the words "For pets". (Bug fix: the For pets section shared a style name with the pet portraits, so its heading sat beside the list instead of above it.) |
| 9 | Put the pets images to the right of the logo and give big pictures of cuteness. |
| 10 | 24/7 delivery to anywhere in the world - we do not ship pets only food! PUSH |
| 11 | Delivery anywhere in the world, not pickup... we delivery food... pet's welcome needs to be a bigger part of the main banner. PUSH |

## Main features

- **Sweet and savory lists:** 17 items in list form, grouped into Sweet (pastries, cookies and bars, whole cakes), Savory (breads, bagels and kolaches), and For pets, with filter buttons for All, Sweet, Savory, and For pets.
- **Color theme:** ivory and beige background with orange and blue accents. The page stays ivory even when a device is set to dark mode.
- **Pets welcome banner:** a large "Pets welcome!" headline in the header, with a line on worldwide 24/7 delivery and a note that the bakery delivers food, not pets.
- **Logo:** the Corner Crumb Bakery logo replaces the text title in the header (`images/logo.png`).
- **Pet portraits:** four big round pet portraits (Labrador, orange tabby, gray and white cat, terrier) to the right of the logo, shown large (128 px on desktop, smaller on phones), saved in `images/`.
- **Pet treats:** dog biscuits, a carrot pupcake, sweet potato chews, and a barkday cake (48 hours' notice), each labeled as made for dogs with no chocolate, xylitol, or raisins.
- **Quantities:** plus and minus buttons or typed numbers; limit of 24 per item (3 per cake).
- **Baker's dozen pricing:** every 13th bagel is free.
- **Running order total:** updates as items change.
- **Delivery only:** delivery anywhere in the world, 24/7, with an address form (street, city, state or region, postal code, country). Delivery costs $8.00 in the US and $35.00 everywhere else; the fee is its own line in the total. No pickup.
- **Date and time:** open 24 hours, 7 days a week; dates from today to 14 days out; 30-minute slots around the clock (12:00 AM to 11:30 PM).
- **Notice rules:** orders need 2 hours' notice; whole cakes, the barkday cake, and international deliveries need 48 hours, so earlier time slots disappear when a cake is in the order.
- **Contact info:** name and phone required (7 to 15 digits, so international numbers work); optional notes for the baker.
- **Review before submitting:** a summary page with Edit order and Place order; placing the order gives an order number.

## Three tests

1. **Totals, baker's dozen, and delivery fee.** Add 2 Butter croissants and 13 Plain bagels. Expected total with US delivery: $8.50 + $21.00 + $8.00 = **$37.50**, with "1 free (baker's dozen)" under the bagels. Change Country to Another country: the total should become **$64.50**.
2. **Delivery time rules.** Choose today: the first time listed should be at least 2 hours from now, and later dates should show slots all day and night, including overnight times like 2:00 AM. Then add an 8-inch carrot cake (or change Country to Another country) and choose tomorrow: no time slots earlier than 48 hours from now should appear.
3. **Review and submit.** Click Review order with an empty order, no address, and no contact info: error messages should list what is missing. Fill everything in, click Review order, check that the summary matches, click Edit order to confirm nothing was lost, then Place order and confirm an order number appears.

## Limits

This is a front-end prototype. Orders are not sent or saved anywhere; there is no payment, inventory, delivery tracking, or bakery-side view.
