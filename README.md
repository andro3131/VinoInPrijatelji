# Vino & Prijatelji

Promocijska spletna stran za degustacijski dogodek **Vino & Prijatelji** - 18. april 2026, Catez pri Trebnjem.

## Tech stack

- [Astro](https://astro.build) - Static site generator
- [Tailwind CSS v4](https://tailwindcss.com) - Styling
- [Stripe Payment Links](https://stripe.com/payments/payment-links) - Prodaja vstopnic

## Ukazi

| Ukaz                | Opis                                     |
| :------------------ | :--------------------------------------- |
| `npm install`       | Namesti odvisnosti                       |
| `npm run dev`       | Zazeni dev server na `localhost:4321`    |
| `npm run build`     | Zgradi produkcijsko stran v `./dist/`   |
| `npm run preview`   | Predogled builda pred deployem          |

## Stripe nastavitev

1. Ustvari [Stripe Payment Link](https://dashboard.stripe.com/payment-links) za 49 EUR
2. V `src/components/Pricing.astro` zamenjaj `href="#"` z URL-jem Payment Linka
3. V Payment Link nastavitvah nastavi success URL na `https://tvoja-domena.si/success`

## Hero slika

Zamenjaj placeholder v `Hero.astro` z dejansko drone fotografijo:
1. Dodaj sliko v `public/images/hero.jpg`
2. V `Hero.astro` zamenjaj gradient `div#hero-bg` z `<img>` elementom
