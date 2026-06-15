Theme Design System: Apple Glossy x Bento Grid
This document outlines the core design system for the educational Salla theme, built on top of "Theme Raed". The design language fuses Glassmorphism with a Bento Grid layout, utilizing negative space to emphasize 3D assets.

1. Core Concept & Colors

Dynamic Theming: The theme relies on Salla's Twilight engine CSS variables for colors, allowing merchants to change the primary brand colors via their dashboard.

Color Blobs/Gradients: The background of the main pages will utilize soft, blurred gradients based on the merchant's primary color to enhance the glass effect of the components positioned above them.

2. Glassmorphism UI Elements
   All major components (cards, banners, features) must be wrapped inside a glass container using the following Tailwind CSS utility classes:

Design Element Tailwind Classes Purpose & Effect
Glass Background bg-white/60 dark:bg-black/40
Creates a semi-transparent layer that lets background colors bleed through.

Backdrop Blur backdrop-blur-xl
Applies the core "Apple Glossy" frosted glass depth effect.

Borders border border-white/30 dark:border-white/10
Defines crisp, subtle edges for the glass containers.

Shadows shadow-[0_8px_30px_rgb(0,0,0,0.04)]
Adds depth, separating the glass layer from the background.

Border Radius rounded-3xl
Ensures smooth, large rounded corners fitting the Bento Grid aesthetic.

3. Layout: Bento Grid System
   The layout relies heavily on CSS Grid to create a modular structure:

Responsive Grid: The main wrapper should utilize grid grid-cols-1 md:grid-cols-3 lg:grid-cols-4 to ensure responsiveness across devices.

Card Spanning: Highlighted elements (e.g., featured courses, promo banners) should span multiple columns or rows using md:col-span-2 or row-span-2 to break the visual monotony.

Negative Space: Generous gaps (gap-6 or gap-8) between grid items and comfortable inner padding (p-8) must be used to maintain a premium, uncluttered look.

4. 3D Assets & Imagery

Asset Containers: Inside the glass cards, create flexible centering wrappers (flex items-center justify-center) to house 3D icons and illustrations.

Floating Effect: The generous negative space combined with the glass background will allow these 3D assets to "float" prominently within the UI.
