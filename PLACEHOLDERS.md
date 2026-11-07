# What to replace before publishing

Everything below is a placeholder or an assumption I made so the site looks
finished. Each one is a two-minute change. Use **Find** in Notepad (Ctrl+F).

## 1. Business WhatsApp number - DONE

The site now uses **+256 700 954 642** (`256700954642` in links). Every
"Order on WhatsApp" button opens a chat with that number and a message already
typed, for example:

> Hello MAHACA Sweet Cakes, I would like to order a cake.

Product buttons fill in the item code too, so the customer only has to press send.
The same number appears in the footer of all five pages.

If the number ever changes, replace `256700954642` in every `.html` file and update
the visible `+256 700 954 642` text.

## 2. Email address - DONE

**mahacasweetcakes@gmail.com** is used in the footer of all five pages. Make sure
the group actually creates this account, because the brief requires accounts to be
made with the group email.

## 2b. Payment details - real, updated by the group

`pay.html` now shows **three** methods:

- **Mobile Money Payments: 0700 954 642** - one number for both MTN and Airtel
  customers. (The separate MTN line `0769 864 032` was removed from the site.)
- **Bank:** Centenary Bank, account name MAHACA SWEET CAKES, account **3204792754**
- **Cash on delivery** on campus

There are no SAMPLE labels any more, at the group's request. Note that the brief asks
for sample numbers and a "payments are not active" note, so if your lecturer applies
that rule strictly this is where you would lose the marks - see section 10.

## 3. Images - all currently placeholders

Replace these files in `images/`. Keep the exact same file names, or the site will
show a broken image.

| File | Used for | Suggested size |
|---|---|---|
| `logo.png` | Header and footer on every page, and the browser tab icon | square, at least 400 x 400 |
| `hero.jpg` | Big picture on the Home page | portrait, 1200 x 1500 |
| `product1.jpg` | MSC-001 Classic Vanilla Cake | landscape, 1200 x 900 |
| `product2.jpg` | MSC-002 Chocolate Fudge Cake | landscape, 1200 x 900 |
| `product3.jpg` | MSC-003 Marble Celebration Cake | landscape, 1200 x 900 |
| `product4.jpg` | MSC-004 Red Velvet Cake | landscape, 1200 x 900 |
| `product5.jpg` | MSC-005 Custom Theme Cake | landscape, 1200 x 900 |
| `product6.jpg` | MSC-006 Cupcake Box | landscape, 1200 x 900 |
| `product7.jpg` | MSC-007 Banana Cake Loaf | landscape, 1200 x 900 |
| `product8.jpg` | MSC-008 Event Sheet Cake | landscape, 1200 x 900 |

Keep each picture under about 300 KB so the site loads quickly on mobile data.
If you photograph an AI-generated image, say so in your AI use log.

## 4. Prices - `products.html` (and the featured cards on `index.html`)

I proposed these from the 80,000 working example in the Business Snapshot. **The
group must approve them**, because the brief does not allow invented prices and the
same prices must appear in the WhatsApp catalogue.

| Code | Product | Proposed price |
|---|---|---|
| MSC-001 | Classic Vanilla Cake (6-inch) | 55,000 |
| MSC-002 | Chocolate Fudge Cake (6-inch) | 60,000 |
| MSC-003 | Marble Celebration Cake (8-inch) | 80,000 |
| MSC-004 | Red Velvet Cake (8-inch) | 90,000 |
| MSC-005 | Custom Theme Cake (8-inch) | 110,000 |
| MSC-006 | Cupcake Box (6) | 25,000 |
| MSC-007 | Banana Cake Loaf | 20,000 |
| MSC-008 | Event Sheet Cake (10-inch) | 150,000 |

If you change a price, change it **everywhere**: `products.html`, the three featured
cards on `index.html`, the WhatsApp catalogue and any social post that shows it.

## 5. Delivery, hours and notice periods

These are on `index.html` (quick facts), `pay.html`, `policies.html` and
`products.html`. Current values:

- delivery within MUBS Jinja Campus: **UGX 5,000**
- collection: **free**
- notice: **24 hours** standard, **48 hours** custom
- hours: **Mon-Sat, 8:00 am - 7:00 pm**, Sunday by arrangement
- order records kept: **six months**

Confirm these with the group and the person handling deliveries.

## 6. Founder roles - `about.html`

The "Who does what" list is a **suggested split** for six people covering the
brief's ten roles. Change it to match the group's real contribution log:

- Mebra - group leader and business planning
- Allan - website builder and payments
- Hazrat - social media and content
- Aisha - marketing plan and content
- Christine - Google profile and WhatsApp catalogue
- Alvin - rules, security and presentation

## 7. Bank details - `pay.html`

Currently "Sample Bank Uganda", account name "MAHACA SWEET CAKES (SAMPLE)" and
account number `0000 0000 0000`. Leave as samples unless the group opens a real
account. The brief says no real money should move.

## 8. Domain name

The site is hosted on GitHub Pages, so the free address will be
`https://<account>.github.io/mahaca-sweet-cakes/`. Task 6 asks which address you
**would** buy and why. Suggested answer for the write-up:

> We would buy `mahacasweetcakes.co.ug`. The `.co.ug` ending shows customers that the
> business is Ugandan, which builds trust locally, and it matches our name exactly so
> it is easy to remember and to say on WhatsApp.

## 9. Social media links - waiting for the group

Facebook, YouTube and LinkedIn icons now appear in two places:

- the **footer of every page**, under a "Follow us" label
- the **dark banner on the About page**, under the WhatsApp button

Each one links to `href="#"` for now, so nothing breaks. When the pages exist,
open each `.html` file, search for `aria-label="MAHACA Sweet Cakes on` and replace
the `#` in that link with the real address:

| Icon | Replace `#` with |
|---|---|
| Facebook | `https://www.facebook.com/your-page-name` |
| YouTube | `https://www.youtube.com/@your-channel-name` |
| LinkedIn | `https://www.linkedin.com/company/your-page-name` |

To do it quickly in Notepad: use **Replace All** on the exact line
`href="#" aria-label="MAHACA Sweet Cakes on Facebook"` and so on, file by file.

Keep the icons in the same order (Facebook, YouTube, LinkedIn) so the site looks
consistent, and make sure the profile name, logo and bio match across all three.

## 10. Need to know (no change needed)

- The footer used to say this is a student project for BUC3106 at MUBS. **That line
  was removed at the group's request.** The brief asks for it on every page, so if
  your lecturer applies the rule strictly, put a short line back in the footer of
  all five pages before handing in.
- Payment numbers are still labelled as samples, and `pay.html` still states clearly
  that payments are not active.
- The site has no analytics, no cookies, no forms and no tracking. That is why the
  privacy notice is short.
