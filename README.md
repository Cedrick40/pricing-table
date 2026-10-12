# Responsive Pricing Table

A static, responsive, single-page pricing table with three plans, built for Task 12 (Pricing Table) of my Web Development internship.

**Live page:** https://cedrick40.github.io/pricing-table/

## About the project
The page shows three hosting plans, Starter, Business and Enterprise. Each card has a price, a feature list and a call-to-action button. The Business plan is highlighted as the most popular one, and the cards stack on small screens.

## Objective
To practice CSS Flexbox/Grid layouts and hover effects.

## Tools used
- HTML5
- CSS3
- VS Code
- Git and GitHub (free)

## My approach
- **Planning:** I decided on a product to sell (web hosting), then wrote the plan names, prices and features before writing any code.
- **Semantic HTML:** I used `main`, `header`, `section` and `article` so each plan is its own meaningful block. The `section` has an `aria-label` for screen readers, and each plan name is an `h2`.
- **Layout with Grid:** I used CSS Grid (`grid-template-columns: repeat(3, 1fr)`) to place the three cards side by side with equal widths and a consistent gap.
- **Layout with Flexbox:** Each card is a flex column. The feature list uses `flex: 1` to take up the spare space, so all three buttons line up at the bottom even when the lists have different lengths.
- **Highlighted plan:** I used a `.popular` class to give the Business card a dark background, a gold border, a stronger `box-shadow`, a slight scale-up and a "Most popular" badge.
- **Hover effects:** The cards lift up and get a deeper shadow on hover. The buttons fill with colour and move up slightly. I also added a visible `:focus-visible` outline for keyboard users and turned off transitions for people who prefer reduced motion.
- **Responsive design:** A media query for screens of 860px and below changes the grid to one column so the cards stack. The popular plan moves to the top on small screens, and the scale-up is removed so nothing scrolls sideways.
- **Testing:** I resized the browser and used the browser's mobile view to check that the cards stack, the text stays readable and nothing scrolls sideways.

## Project structure
```
pricing-table/
├── index.html
├── style.css
└── README.md
```

## Outcome
The result is a clean, responsive pricing table with three plan cards, a highlighted popular plan and responsive stacking on small screens. This project taught me how Grid handles the overall layout while Flexbox aligns the content inside each card, and how hover effects make a page feel interactive.

## Interview questions
- **How would you highlight one plan over the others?** I would use a contrasting background or border colour, a stronger shadow, a slight scale-up and a badge such as "Most popular".
- **What CSS properties create a card shadow?** `box-shadow`, for example `box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);`.
- **How does Flexbox distribute space between items?** Along the main axis, `justify-content` (such as `space-between`) and `gap` control spacing, and `flex-grow` shares leftover space between items.

## Credits
Plan names, prices and features are made-up sample content. The font is Bricolage Grotesque from Google Fonts.

## Author
Cedrick Niyibikora