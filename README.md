# Food Score

**What does it cost to eat 2,000 calories of this?**

A tiny, mobile-first calculator that turns any food label into one comparable number: dollars per 2,000 calories. Spin the wheels — servings, calories per serving, price — and the score updates instantly.

## Why

Price tags tell you cost per package. Labels tell you calories per serving. Neither tells you what actually matters when comparing foods as fuel: **cost per calorie**. Normalizing to 2,000 calories (a typical daily intake) gives every food a common denominator:

- Rice at $1.20 per 2,000 cal and frozen pizza at $6.80 per 2,000 cal are now directly comparable.
- Green (< $2.50) / orange / red (≥ $8.00) bar gives an at-a-glance verdict.

## The math

```
cost per 2,000 cal = 2000 / (calories × servings) × price
```

Example: 15 servings × 80 cal = 1200 calories per package, at $2.40
→ `2000 / 1200 × 2.40` = **$4.00** per 2,000 calories.

## Usage

Open `index.html`. That's it — no build, no install, no dependencies, no network.

- **Spin** the wheels like an iPhone alarm clock (servings 1–20, calories 20–1000, price in dollars + 5¢ increments; the cents wheel loops endlessly).
- **Tap** the selected value to type it directly.
- The score and color bar update live as you spin.

Works offline; nothing is stored or sent anywhere.

## License

MIT
