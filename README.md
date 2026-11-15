# Drinks Shop App

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Supatmo Cahyono** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `drinks-shop-app-concept-supatmo-cahyono.sketch` by **Supatmo Cahyono**: one route per artboard, with the artboard's layout, colours, images and text.

![Drinks Shop App screens](./showcase.jpg)

## 📱 Screens (15 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **01 - Splash** · start screen | `src/app/s-01-splash.jsx` | 375 × 667 | 1 |
| 2 | **01 - Cart** | `src/app/s-01-cart.jsx` | 375 × 667 | 4 |
| 3 | **01 - Slide Category Taro** | `src/app/s-01-slide-category-taro.jsx` | 375 × 667 | 2 |
| 4 | **03 - Checkout (Delivery)** | `src/app/s-03-checkout-delivery.jsx` | 375 × 667 | 2 |
| 5 | **04 - Slide Category Espresso** | `src/app/s-04-slide-category-espresso.jsx` | 375 × 667 | 2 |
| 6 | **02 - Cart (Delete Item)** | `src/app/s-02-cart-delete-item.jsx` | 375 × 667 | 4 |
| 7 | **03 - Checkout (Delivery) Null** | `src/app/s-03-checkout-delivery-null.jsx` | 375 × 667 | 3 |
| 8 | **04 - Slide Category Espresso (Selected)** | `src/app/s-04-slide-category-espresso-selected.jsx` | 375 × 667 | 3 |
| 9 | **02 - Cart (Empty)** | `src/app/s-02-cart-empty.jsx` | 375 × 667 | 2 |
| 10 | **03 - Slide Category Green** | `src/app/s-03-slide-category-green.jsx` | 375 × 667 | 2 |
| 11 | **05 - Checkout (Payment)** | `src/app/s-05-checkout-payment.jsx` | 375 × 667 | 3 |
| 12 | **02 - Slide Category Thai** | `src/app/s-02-slide-category-thai.jsx` | 375 × 667 | 2 |
| 13 | **03 - Slide Category Green (Added to Bag)** | `src/app/s-03-slide-category-green-added-to-bag.jsx` | 375 × 667 | 3 |
| 14 | **05 - Slide Category Java Tea** | `src/app/s-05-slide-category-java-tea.jsx` | 375 × 667 | 2 |
| 15 | **04 - Checkout (Payment)** | `src/app/s-04-checkout-payment.jsx` | 375 × 667 | 3 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Poppins), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/drinks-shop-app> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **Drinks App with Checkout** design by **Supatmo Cahyono**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Supatmo Cahyono](https://www.sketchappsources.com/contributor/supatmocahyono) |
| Original design | [Drinks App with Checkout](https://dribbble.com/shots/6759784-Segertea-App-Drinks-Shop-Simple-App-UI-Kit) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4068-drinks-shop-app-concept-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/bungmomo> |
| Original file | `drinks-shop-app-concept-supatmo-cahyono.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "Drinks App with Checkout" by Supatmo Cahyono (https://dribbble.com/shots/6759784-Segertea-App-Drinks-Shop-Simple-App-UI-Kit), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4068-drinks-shop-app-concept-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
