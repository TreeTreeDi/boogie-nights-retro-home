---
version: alpha
name: Boogie Nights Retro Home
iteration: 1.0.0
description: A retro boho, mid-century modern landing page identity for a warm home styling / lifestyle commerce website. Built for AI coding agents and frontend implementation.
colors:
  cream: "#F6E8C7"
  cream-soft: "#FFF3D3"
  caramel-bg: "#C6955A"
  burnt-orange: "#C95508"
  burnt-orange-dark: "#9F3F04"
  mustard: "#F7B900"
  teal: "#5BAE9A"
  teal-dark: "#3D8878"
  forest-green: "#4F9275"
  cocoa: "#4A2C1B"
  espresso: "#24140D"
  white-warm: "#FFF9EA"
  black-soft: "#17110C"
  border-orange: "#F39800"
  shadow-warm: "rgba(36, 20, 13, 0.28)"
typography:
  logo:
    fontFamily: "Cooper Black, Fraunces, Georgia, serif"
    fontSize: 40px
    fontWeight: 800
    lineHeight: 1
    letterSpacing: -0.02em
  display-xl:
    fontFamily: "Cooper Black, Fraunces, Georgia, serif"
    fontSize: 96px
    fontWeight: 900
    lineHeight: 0.88
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: "Cooper Black, Fraunces, Georgia, serif"
    fontSize: 56px
    fontWeight: 800
    lineHeight: 1.02
    letterSpacing: -0.03em
  headline-md:
    fontFamily: "Cooper Black, Fraunces, Georgia, serif"
    fontSize: 36px
    fontWeight: 800
    lineHeight: 1.08
    letterSpacing: -0.02em
  body-lg:
    fontFamily: "Inter, Public Sans, Arial, sans-serif"
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.65
  body-md:
    fontFamily: "Inter, Public Sans, Arial, sans-serif"
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.65
  body-sm:
    fontFamily: "Inter, Public Sans, Arial, sans-serif"
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.55
  label-caps:
    fontFamily: "Inter, Public Sans, Arial, sans-serif"
    fontSize: 11px
    fontWeight: 800
    lineHeight: 1
    letterSpacing: 0.16em
  script-accent:
    fontFamily: "Lobster, Pacifico, cursive"
    fontSize: 28px
    fontWeight: 400
    lineHeight: 1.1
rounded:
  none: 0px
  sm: 4px
  md: 8px
  lg: 14px
  xl: 22px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  2xl: 64px
  3xl: 96px
  page-x: 7vw
  section-y: 96px
  gutter: 32px
components:
  page:
    backgroundColor: "{colors.caramel-bg}"
    textColor: "{colors.espresso}"
  content-shell:
    backgroundColor: "{colors.cream}"
    width: "min(100%, 1440px)"
    shadow: "0 34px 90px {colors.shadow-warm}"
  hero:
    backgroundColor: "{colors.espresso}"
    textColor: "{colors.white-warm}"
    minHeight: 720px
  nav:
    textColor: "{colors.white-warm}"
    typography: "{typography.label-caps}"
    height: 76px
  button-primary:
    backgroundColor: "{colors.mustard}"
    textColor: "{colors.espresso}"
    typography: "{typography.label-caps}"
    rounded: "{rounded.md}"
    padding: "14px 28px"
  button-primary-hover:
    backgroundColor: "#FFCA1A"
    textColor: "{colors.espresso}"
  brand-strip:
    backgroundColor: "{colors.teal}"
    textColor: "{colors.white-warm}"
    height: 82px
  photo-frame:
    borderColor: "{colors.border-orange}"
    backgroundColor: "{colors.mustard}"
    borderWidth: 8px
    shadow: "0 18px 38px rgba(74, 44, 27, 0.18)"
  orange-section:
    backgroundColor: "{colors.burnt-orange}"
    textColor: "{colors.white-warm}"
  testimonial-section:
    backgroundColor: "{colors.cream-soft}"
    textColor: "{colors.espresso}"
---

# Boogie Nights Retro Home DESIGN.md

## Overview

This interface should feel like a warm retro home store, not a generic modern SaaS page. The visual language is mid-century, boho, cozy, editorial, and a little playful. It should look like a lovingly styled vintage apartment: wood grain, brick texture, cream paper backgrounds, rounded groovy typography, mustard CTAs, teal brand strips, orange editorial panels, framed photos, flower stickers, and sparkle accents.

The product should feel personal and handcrafted. Avoid a clean corporate look. The page can be polished, but it should still feel tactile, imperfect, and lived-in. Use large nostalgic headlines, oversized decorative words, asymmetrical image placement, thick colored frames, and warm photographic assets.

Primary use case: frontend implementation of a full-page landing page for a retro home styling / vintage lifestyle brand. The first implementation target is desktop web / macOS browser width, with responsive behavior down to tablet and mobile.

## Colors

The palette is built from warm cream, burnt orange, teal, mustard yellow, and deep espresso brown.

Cream is the main canvas. Use `cream` or `cream-soft` for most page backgrounds. It should feel like aged paper rather than pure white.

Burnt orange is the strongest section color. Use it for large editorial blocks, footers, dividers, and warm emphasis areas. Do not use it for every button; buttons should stay mustard unless there is a strong reason.

Teal is the balancing cool color. Use it for the press strip, small dots, secondary marks, and occasional label treatments.

Mustard is the primary action color. Use it for CTA buttons, small highlight chips, and selective graphic accents.

Espresso and cocoa are the text and shadow colors. Avoid pure black unless needed for accessibility or image overlays.

Recommended text contrast pairings:

- `espresso` text on `cream`, `cream-soft`, or `mustard`.
- `white-warm` text on `burnt-orange`, `burnt-orange-dark`, or dark image overlays.
- `white-warm` text on `teal` for brand-strip labels.
- `forest-green` for large headlines on cream backgrounds when a softer tone is desired.

## Typography

Typography is the main personality driver. Use a chunky groovy serif for logo, hero headings, section headings, and oversized decorative display text. Good implementation choices are Cooper Black, Fraunces Black, or a similar 1970s-inspired serif. If the exact display font is unavailable, use `Fraunces` or `Georgia` as fallback, but keep weight heavy and letter spacing slightly tight.

Use clean sans-serif text for body copy, navigation, labels, buttons, and metadata. Inter or Public Sans works well. Body copy should stay readable and not become overly stylized.

Use all-caps labels with wide letter spacing for nav items, eyebrow text, brand-strip metadata, and button text. This creates contrast against the soft rounded headline style.

Large typography rules:

- Hero headline should be big, centered, and layered over photography.
- Section headlines should be large and slightly compressed vertically.
- Decorative words, such as “REVIEWS”, can be enormous and partially placed behind content, but they must never block readability.
- Avoid more than two primary font families per screen, excluding optional script/neon text inside photographic assets.

## Layout

Use a centered page shell on a warm caramel outer background. The main site content should feel like a vertical editorial poster inside the browser. On desktop, the shell can be full width up to 1440px. The outer caramel background and soft shadow are part of the presentation when showing the design as a mockup.

The layout should move from top to bottom like this:

1. Full-bleed hero image with nav overlay and centered headline.
2. Teal “as seen in” brand strip.
3. Cream editorial intro section with floating framed interior photos and flower/sparkle accents.
4. Founder section with a large framed portrait on the left and text on the right.
5. Burnt orange product/package section with copy on the left and a warm interior image on the right.
6. Cream testimonial section with oversized background display typography and a framed portrait.
7. Burnt orange footer with small links and social icons.

Desktop content should use a generous grid, but it should not feel rigid. Use intentional offsets: one photo higher, another photo pulled to the edge, a flower partially outside the section boundary. The composition should feel curated rather than symmetrical.

Spacing should be generous between major sections. Internal content blocks can be tighter, but never cramped. Images should have breathing room and visible frame treatment.

Responsive behavior:

- Desktop: preserve editorial asymmetry and overlapping decorative elements.
- Tablet: reduce oversized type and simplify image offsets.
- Mobile: stack content vertically, remove risky overlaps, keep one strong image per section, and ensure CTAs remain visible above long copy.

## Elevation & Depth

Depth should come from photography, frames, warm shadows, and layered decorative objects. Use soft shadows, never cold gray shadows.

Use `photo-frame` for key images. The frame can be mustard or orange with a thin darker edge. The image should feel like a physical poster or framed print sitting on top of the cream background.

The main page shell can cast a large warm shadow when presented inside a mockup canvas. Inside the page, use fewer shadows and rely on color blocking, image framing, and typography scale.

Image overlays in the hero should use a dark warm gradient so white headline text remains readable without making the photo feel dull.

## Shapes

The shape system should be mostly rectangular with subtle softness. This is not a pill-heavy modern app. Use small radii on buttons and cards. Photos can be sharp rectangles with thick frames. Decorative dots and flower petals should be fully rounded.

Buttons use a small radius, not a pill, to keep the retro poster feel. Navigation cart button may use slightly more rounding, but should still feel compact.

The brand’s decorative shapes are flowers, dots, sparkles, and large organic type. Do not introduce unrelated abstract blobs unless they match the flower/paper-cut aesthetic.

## Components

Navigation should be placed over the hero image. Logo sits left, nav links centered or left-center, cart action right. Links are uppercase, small, and spaced out. On mobile, collapse into a simple menu icon while keeping the logo visible.

Hero should use a high-quality warm interior photo, full bleed. Add a dark warm overlay. Center the headline and CTA. The CTA should be mustard with espresso text.

Brand strip should be teal, horizontally aligned, and compact. Use white text/logotypes. Do not over-design this area; it is a rhythm break between image and cream content.

Photo cards should use thick mustard/orange borders. Use editorial crops: one vertical product/interior crop, one cozy corner crop, one founder portrait, one package/product environment image, and one testimonial portrait.

Founder block should combine a framed portrait with a headline in green. Keep the copy short and friendly. Use a small uppercase eyebrow above the headline.

Package section should be burnt orange and image-led. Copy should be white or warm cream. CTA remains mustard.

Review section should use the huge word “REVIEWS” as a background layer in warm white. The testimonial card sits over it. Keep the testimonial legible and avoid placing body copy directly over complex decorative type.

Footer should be simple, burnt orange, and low-contrast but readable. Use small uppercase links and minimal social icons.

## Assets

Use assets as frontend materials rather than single flattened screenshots.

Required assets from top to bottom:

- `logo-boogie-nights-transparent.png`: transparent-background wordmark for header and footer.
- `hero-living-room.jpg`: wide mid-century living room with brick wall, wood furniture, bookshelves, plants, warm rug, and red daybed.
- `decor-lamp-cabinet.jpg`: vertical crop of wooden cabinet, warm lamp, plant, and wall shelf.
- `decor-reading-corner.jpg`: vertical cozy chair / book corner crop.
- `founder-red-suit.jpg`: founder-style portrait in red outfit against circular bookshelf.
- `package-neon-interior.jpg`: warm brick-wall product/package scene with red fridge and neon sign.
- `testimonial-portrait-yellow.jpg`: smiling portrait on mustard/yellow background.
- `flower-orange.svg`: flat retro orange flower with rounded petals.
- `sparkles-orange.svg`: small four-point sparkle cluster.
- `dot-pair.svg`: stacked orange and teal circular dots.

Asset treatment rules:

- Photos should be warm, slightly saturated, and editorial.
- Do not mix cold blue photography into this design.
- Do not use generic stock-photo office imagery.
- Human portraits should feel like founder/customer/editorial portraits, not corporate headshots.
- Logo should be used as image or SVG when possible; if implemented as text, match `typography.logo`.

## Accessibility

Maintain WCAG AA contrast for body text and buttons. Large decorative typography can be lower contrast when it is non-essential, but actual copy must remain readable.

Never place small body text directly on busy photography without an overlay or solid backing. Hero text must have a dark gradient overlay behind it.

Buttons must have visible focus states. Use a dark espresso outline or a high-contrast inset focus ring. Interactive elements need at least 44px target height on touch devices.

## Do's and Don'ts

Do make the page feel warm, nostalgic, personal, and styled.

Do use cream, burnt orange, teal, mustard, and espresso as the core palette.

Do use large groovy typography and thick framed photography.

Do use asymmetry intentionally, especially on desktop.

Do keep CTAs mustard and easy to find.

Don't make the page look like a SaaS dashboard or minimalist portfolio.

Don't use pure white backgrounds as the main canvas.

Don't add glassmorphism, neon cyberpunk gradients, blue-purple tech colors, or generic card grids.

Don't overuse shadows; frames, color blocks, and photo depth should carry the composition.

Don't let decorative text, flowers, or sparkles cover meaningful content.

## Frontend Implementation Notes

Recommended stack mapping:

- CSS variables should be generated from the YAML color and spacing tokens.
- Tailwind users can map colors directly into `theme.extend.colors`.
- Use `clamp()` for headings so desktop retains drama while mobile remains readable.
- Use CSS grid for editorial desktop sections and switch to single-column flex/grid on mobile.
- Use `object-fit: cover` and deliberate `object-position` for photo crops.
- Use pseudo-elements for oversized decorative words and sparkle clusters when they do not need to be separate DOM content.

Suggested CSS variable prefix: `--bn-*`, for example `--bn-cream`, `--bn-orange`, `--bn-teal`, `--bn-mustard`, `--bn-espresso`.
