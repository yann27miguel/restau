# restau
My goal was to master tailwind CSS using a project to learn . i created a high-end, multilingual and responsive restaurant landing page using strictly HTML and Tailwind CSS -with zero javascript

This project was a hands-on deep dive into utility-first CSS architecture. Instead of relying on pre-built UI component libraries or JavaScript frameworks for interactive states, I pushed Tailwind’s utility classes, state variants, and arbitrary value extensions to their limits.

Building L'Étoile Fine Dining taught me how to replace traditional CSS stylesheets with composable atomic classes while keeping the design cohesive, performant, and accessible.

💡 Core Tailwind CSS Concepts & Highlights
Here are the key Tailwind classes and techniques that powered this project:

1. Custom Design Tokens & Arbitrary Values
To achieve a bespoke luxury aesthetic rather than standard default colors, I made extensive use of Tailwind's arbitrary value syntax [value] and customized color extensions:

Backgrounds & Accents: bg-[#0a0a0c] (obsidian charcoal) and text-[#c5a059] / bg-[#c5a059] (brushed gold) gave the entire website its high-contrast Michelin-guide atmosphere.

Fine Spacing & Borders: border-[#c5a059]/20 (border with 20% opacity) and tracking-[0.25em] (custom wide letter-spacing for editorial headings).

2. Layouts, Grid Systems & Responsiveness
Managing clean spacing across mobile and widescreen viewports using responsive modifiers:

Responsive Multi-columns: grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 ensured dish cards and accolades fluidly adapt from a single stacked column on phones to 3 columns on desktop.

Sticky Positioning & Headers: sticky top-0 z-50 backdrop-blur-md bg-[#0a0a0c]/90 keeps the navigation bar fixed with an elegant frosted-glass blur effect as visitors scroll down.

Centering & Flow: max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 creates consistent alignment and viewport gutters across all sections.

3. Micro-Interactions Without JavaScript
Interactive states were handled purely with Tailwind’s pseudo-class variants:

Hover & Transitions: transition-all duration-500 ease-out hover:scale-105 hover:border-[#c5a059]/40 adds fluid micro-animations to menu cards and gallery photos.

Group Hovering: Pairing group on parent containers with group-hover:text-[#c5a059] on children allowed nested elements (like dish names and price tags) to animate simultaneously when a user hovers anywhere over the card.

Form Focus States: focus:outline-none focus:border-[#c5a059] focus:ring-1 focus:ring-[#c5a059] provides tactile feedback on inputs while maintaining brand palette harmony.

4. The Zero-JS Language Switcher (Peer & Sibling States)
The most challenging part of the project was switching between English, French, and German without JavaScript:

By using hidden semantic `` elements, I utilized CSS sibling selectors and Tailwind utility classes (hidden, `block`, and custom CSS rules) to dynamically display and hide text blocks (`.en-text`, `.fr-text`, `.de-text`) depending on which radio pill is active.
