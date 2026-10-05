# airbnb DESIGN.md

> Auto-generated design system — reverse-engineered via static analysis by skillui.
> Frameworks: None detected
> Colors: 20 · Fonts: 3 · Components: 6
> Icon library: not detected · State: not detected
> Primary theme: light · Dark mode toggle: yes · Motion: expressive

## Visual Reference

**Match this design exactly** — study colors, fonts, spacing, and component shapes before writing any UI code.

![airbnb Homepage](../screenshots/homepage.png)

---

## 1. Visual Theme & Atmosphere

This is a **light-themed** interface with a warm, approachable feel. The light background emphasizes content clarity. Typography pairs **Roboto** for display/headings with **kakaopay System Sans** for body text, creating clear visual hierarchy through type contrast. Spacing follows a **4px base grid** (compact density), with scale: 2, 4, 6, 8, 10, 12, 14, 16px. The accent color **#ff385c** anchors interactive elements (buttons, links, focus rings). Motion is expressive — spring physics, layout animations, and staggered reveals are part of the visual language.

---

## 2. Color Palette & Roles

| Token | Hex | Role | Use |
|---|---|---|---|
| theme-color | `#ffffff` | background | Page background, darkest surface |
| palette-bg-primary-disabled | `#f2f2f2` | surface | Card and panel backgrounds |
| palette-bg-primary-luxe | `#222222` | text-primary | Headings and body text |
| dls-button_background_disabled | `#4a4a4a` | text-muted | Captions, placeholders, secondary info |
| palette-text-secondary | `#6c6c6c` | text-muted | Captions, placeholders, secondary info |
| palette-bg-primary-inverse-hover | `#3f3f3f` | border | Dividers, card borders, outlines |
| palette-bg-primary-core | `#ff385c` | accent | CTAs, links, focus rings, active states |
| palette-bg-primary-inverse-error-hover | `#a3150f` | danger | Error states, destructive actions |
| palette-text-success | `#038026` | success | Success states, positive indicators |
| info | `#008489` | info | Informational highlights |
| elevation-sharp-edge-background | `#000000` | unknown | Palette color |
| palette-bg-beige-secondary-hover | `#c1c1c1` | unknown | Palette color |
| palette-bg-primary-inverse-disabled | `#dddddd` | unknown | Palette color |
| dls-button_color_disabled | `#878787` | unknown | Palette color |
| palette-bg-primary-inverse-invalid | `#d7251c` | unknown | Palette color |
| palette-bg-primary-inverse-error | `#c13515` | unknown | Palette color |
| palette-bg-primary | `#111111` | unknown | Palette color |
| palette-text-brand-selected | `#da1249` | unknown | Palette color |
| palette-bg-primary-selected | `#2c2c2c` | unknown | Palette color |
| palette-bg-primary-inverse-error | `#e74d2e` | unknown | Palette color |

### Dark Mode Token Mapping

| Variable | Light | Dark |
|---|---|---|
| `--elevation-high-box-shadow` | `0 8px 28px rgba(0,0,0,0.28)` | `var(--elevation-high-box-shadow-dark)` |
| `--elevation-high-border` | `1px solid rgba(0,0,0,0.04)` | `var(--elevation-high-border-dark)` |
| `--elevation-primary-box-shadow` | `0 6px 20px rgba(0,0,0,0.2)` | `var(--elevation-primary-box-shadow-dark)` |
| `--elevation-primary-border` | `1px solid rgba(0,0,0,0.04)` | `var(--elevation-primary-border-dark)` |
| `--elevation-secondary-box-shadow` | `0 6px 16px rgba(0,0,0,0.12)` | `var(--elevation-secondary-box-shadow-dark)` |
| `--elevation-secondary-border` | `1px solid rgba(0,0,0,0.04)` | `var(--elevation-secondary-border-dark)` |
| `--elevation-sharp-edge-background` | `rgba(0,0,0,0.08)` | `var(--elevation-sharp-edge-background-dark)` |
| `--elevation-tertiary-box-shadow` | `0 2px 4px rgba(0,0,0,0.18)` | `var(--elevation-tertiary-box-shadow-dark)` |
| `--elevation-tertiary-border` | `1px solid rgba(0,0,0,0.08)` | `var(--elevation-tertiary-border-dark)` |
| `--elevation-elevation0-box-shadow` | `0px 0px 0px 1px #DDDDDD inset` | `var(--elevation-elevation0-box-shadow-dark)` |
| `--elevation-elevation1-box-shadow` | `0px 0px 0px 1px color-mix(in srgb,#000000 2%,transparent),0px 2px 4px 0px color-mix(in srgb,#000000 16%,transparent)` | `var(--elevation-elevation1-box-shadow-dark)` |
| `--elevation-elevation2-box-shadow` | `0px 0px 0px 1px color-mix(in srgb,#000000 2%,transparent),0px 2px 6px 0px color-mix(in srgb,#000000 4%,transparent),0px 4px 8px 0px color-mix(in srgb,#000000 10%,transparent)` | `var(--elevation-elevation2-box-shadow-dark)` |
| `--elevation-elevation3-box-shadow` | `0px 0px 0px 1px color-mix(in srgb,#000000 2%,transparent),0px 8px 24px 0px color-mix(in srgb,#000000 10%,transparent)` | `var(--elevation-elevation3-box-shadow-dark)` |
| `--elevation-elevation4-box-shadow` | `0px 0px 0px 1px color-mix(in srgb,#000000 2%,transparent),0px 4px 8px 0px color-mix(in srgb,#000000 8%,transparent),0px 12px 30px 0px color-mix(in srgb,#000000 18%,transparent)` | `var(--elevation-elevation4-box-shadow-dark)` |
| `--elevation-elevation5-box-shadow` | `0px 0px 0px 1px color-mix(in srgb,#000000 2%,transparent),0px 6px 8px 0px color-mix(in srgb,#000000 8%,transparent),0px 16px 56px 0px color-mix(in srgb,#000000 18%,transparent)` | `var(--elevation-elevation5-box-shadow-dark)` |
| `--palette-bg-primary` | `#FFFFFF` | `var(--palette-bg-primary-dark)` |
| `--palette-bg-primary-disabled` | `#F2F2F2` | `var(--palette-bg-primary-disabled-dark)` |
| `--palette-bg-primary-hover` | `#F7F7F7` | `var(--palette-bg-primary-hover-dark)` |
| `--palette-bg-primary-selected` | `#F7F7F7` | `var(--palette-bg-primary-selected-dark)` |
| `--palette-bg-primary-error` | `#FFF5F3` | `var(--palette-bg-primary-error-dark)` |

### CSS Variable Tokens

```css
--amplify-colors-brand-primary-10: var(--palette-rausch100);
--amplify-colors-brand-primary-20: var(--palette-rausch200);
--amplify-colors-brand-primary-40: var(--palette-rausch400);
--amplify-colors-brand-primary-60: var(--palette-rausch600);
--amplify-colors-brand-primary-80: var(--palette-rausch700);
--amplify-colors-brand-primary-90: var(--palette-rausch800);
--amplify-colors-brand-primary-100: var(--palette-rausch900);
--amplify-colors-primary-10: var(--palette-rausch100);
--amplify-colors-primary-20: var(--palette-rausch200);
--amplify-colors-primary-40: var(--palette-rausch400);
--amplify-colors-primary-60: var(--palette-rausch600);
--amplify-colors-primary-80: var(--palette-rausch600);
--amplify-colors-primary-90: var(--palette-rausch800);
--amplify-colors-primary-100: var(--palette-rausch900);
--amplify-colors-background-primary: var(--palette-bg-primary);
--amplify-colors-background-secondary: var(--palette-bg-secondary);
--amplify-colors-font-primary: var(--palette-text-primary);
--amplify-colors-font-secondary: var(--palette-text-secondary);
--amplify-colors-border-primary: var(--palette-border-primary);
--amplify-colors-border-tertiary: var(--palette-border-tertiary);
```


---

## 3. Typography Rules

**Font Stack:**
- **kakaopay System Sans** — Heading 1, Heading 2, Heading 3
- **Roboto** — Body, Caption
- **SFMono-Regular** — Code

**Font Sources:**

```css
@font-face {
  font-family: "Airbnb Cereal VF";
  src: url("https://a0.muscache.com/airbnb/static/airbnb-dls-web/build/fonts/cereal-variable/AirbnbCerealVF_W_Wght.8816d9e5c3b6a860636193e36b6ac4e4.woff2") format("woff2 supports variations");
  font-weight: 400;
}
```

| Role | Font | Size | Weight |
|---|---|---|---|
| Heading 1 | kakaopay System Sans | 9.0625rem | 700 |
| Heading 2 | kakaopay System Sans | 7.5rem | 700 |
| Heading 3 | kakaopay System Sans | 6.25rem | 700 |
| Body | Roboto | 0.875rem | 400 |
| Caption | Roboto | 0.8125rem | 400 |
| Code | SFMono-Regular | 14px | 400 |

**Typographic Rules:**
- Limit to 3 font families max per screen
- Use **kakaopay System Sans** for body/UI text, **Roboto** for display/headings
- Maintain consistent hierarchy: no more than 3-4 font sizes per screen
- Headings use bold (600-700), body uses regular (400)
- Line height: 1.5 for body text, 1.2 for headings
- Use color and opacity for secondary hierarchy, not additional font sizes


---

## 4. Component Stylings

### Navigation (1)

**Navigation** — `html`

### Data Input (2)

**Button** — `html`
- Animation: 

**Input** — `html`
- State: :focus, :placeholder

### Media (3)

**Image** — `html`

**Icon** — `html`

**Map/Canvas** — `html`



---

## 5. Layout Principles

- **Base spacing unit:** 4px
- **Spacing scale:** 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24
- **Border radius:** 0.25rem, 0.5rem, 1px, 1ch, 1rem, 1.5px, 1.875rem, 2px, 3px, 3.2px, 4px, 5.25px, 5.5px, 6px, 8px, 9px, 10px, 11px, 12px, 14px, 14%, 15px, 16px, 17px, 18px, 20px, 22px, 24px, 26px, 27px, 28px, 28%, 29px, 30px, 32px, 36px, 40px, 42px, 42.654px, 44px, 45px, 48px, 50px, 54px, 56px, 80px, 99em, 100px, 100%, 128px, 500px, 999px, inherit, 133px, 1000px, calc(infinity*1px), unset
- **Max content width:** 1127px

**Spacing as Meaning:**
| Spacing | Use |
|---|---|
| 4-8px | Tight: related items within a group |
| 12-16px | Medium: between groups |
| 24-32px | Wide: between sections |
| 48px+ | Vast: major section breaks |


---

## 6. Depth & Elevation

### Flat — subtle depth hints

- `0 0 0 1px var(--palette-grey400) inset`
- `0 0 0 2px var(--palette-grey400) inset`
- `inset 0 0 0 2px red`

### Raised — cards, buttons, interactive elements

- `var(--elevation-elevation1-box-shadow)`
- `var(--elevation-elevation2-box-shadow)`
- `var(--dls_button_box-shadow)`

### Floating — dropdowns, popovers, modals

- `0 6px 20px var(--palette-shadow300)`
- `0 2px 16px var(--palette-shadow150)`
- `0 4px 16px rgba(0,0,0,0.16)`

### Overlay — full-screen overlays, top-level dialogs

- `0 0 0 2000px var(--overlay-box-shadow-color)`
- `0 0 0 2000px rgba(0,0,0,0.5)`
- `0 0 0 30px var(--palette-bg-primary) inset`

### Z-Index Scale

`0, 1, 2, 3, 4, 5, 6, 8, 9, 10, 11, 15, 20, 21, 99, 100, 101, 200, 250, 251, 300, 500, 999, 1000, 1998, 1999, 2000, 2001, 2002, 2003, 2004, 2005, 2100, 3001, 9999, 10000, 10001, 100001, 999999, 10000000, 2147483647, 99999999999`



---

## 7. Animation & Motion

This project uses **expressive motion**. Animations are an integral part of the experience.

### CSS Animations

- `@keyframes kf-s0j3wl`
- `@keyframes kf-h0qfv9`
- `@keyframes kf-1qnooym`
- `@keyframes kf-14dwuik`
- `@keyframes kf-12tey57`
- `@keyframes kf-uo7jbc`
- `@keyframes kf-1dua8o5`
- `@keyframes kf-ogm7kb`

### Animated Components

- **Button**: 

### Motion Guidelines

- Duration: 150-300ms for micro-interactions, 300-500ms for page transitions
- Easing: `ease-out` for enters, `ease-in` for exits
- Always respect `prefers-reduced-motion`


---

## 8. Do's and Don'ts

### Do's

- Use `#ff385c` for interactive elements (buttons, links, focus rings)
- Use `#ffffff` as the primary page background
- Pair **kakaopay System Sans** (body) with **Roboto** (display) — these are the only allowed fonts
- Follow the **4px** spacing grid for all margins, padding, and gaps
- Use the defined shadow tokens for elevation — see Section 6
- Use border-radius from the scale: 0.25rem, 0.5rem, 1px, 1ch, 1rem
- Reuse existing components from Section 4 before creating new ones
- Always use CSS variables for colors — never hardcode hex
- Test both light and dark modes for contrast

### Don'ts

- Don't introduce colors outside this palette — extend the design tokens first
- Don't introduce additional font families beyond kakaopay System Sans and Roboto and SFMono-Regular
- Don't use arbitrary spacing values — stick to multiples of 4px
- Don't create custom box-shadow values outside the system tokens
- Don't use arbitrary border-radius values — pick from the defined scale
- Don't duplicate component patterns — check Section 4 first
- Don't use backdrop-blur or blur effects

### Anti-Patterns (detected from codebase)

- No blur or backdrop-blur effects
- No zebra striping on tables/lists


---

## 9. Responsive Behavior

| Name | Value | Source |
|---|---|---|
| xs | 23em | css |
| xs | 270px | css |
| xs | 300px | css |
| xs | 320px | css |
| xs | 325px | css |
| xs | 330px | css |
| xs | 357px | css |
| xs | 366px | css |
| xs | 370px | css |
| xs | 375px | css |
| xs | 376px | css |
| xs | 395px | css |
| xs | 401px | css |
| xs | 420px | css |
| xs | 429px | css |
| xs | 431px | css |
| xs | 440px | css |
| sm | 499px | css |
| sm | 500px | css |
| sm | 535px | css |
| sm | 541px | css |
| sm | 550px | css |
| sm | 551px | css |
| sm | 599px | css |
| sm | 600px | css |
| sm | 633px | css |
| sm | 634px | css |
| sm | 639px | css |
| sm | 640px | css |
| md | 667px | css |
| md | 679px | css |
| md | 680px | css |
| md | 693px | css |
| md | 694px | css |
| md | 699px | css |
| md | 700px | css |
| md | 743px | css |
| md | 743.99px | css |
| md | 744px | css |
| md | 759px | css |
| md | 760px | css |
| md | 768px | css |
| lg | 777px | css |
| lg | 778px | css |
| lg | 800px | css |
| lg | 813px | css |
| lg | 814px | css |
| lg | 819px | css |
| lg | 820px | css |
| lg | 871px | css |
| lg | 872px | css |
| lg | 879px | css |
| lg | 880px | css |
| lg | 894px | css |
| lg | 909px | css |
| lg | 910px | css |
| lg | 939px | css |
| lg | 940px | css |
| lg | 949px | css |
| lg | 950px | css |
| lg | 959px | css |
| lg | 960px | css |
| lg | 969px | css |
| lg | 970px | css |
| lg | 983px | css |
| lg | 984px | css |
| lg | 1024px | css |
| xl | 1039px | css |
| xl | 1040px | css |
| xl | 1049px | css |
| xl | 1050px | css |
| xl | 1059px | css |
| xl | 1060px | css |
| xl | 1075px | css |
| xl | 1119px | css |
| xl | 1120px | css |
| xl | 1127px | css |
| xl | 1127.99px | css |
| xl | 1128px | css |
| xl | 1140px | css |
| xl | 1141px | css |
| xl | 1159px | css |
| xl | 1160px | css |
| xl | 1189px | css |
| xl | 1190px | css |
| xl | 1194px | css |
| xl | 1199px | css |
| xl | 1200px | css |
| xl | 1227px | css |
| xl | 1228px | css |
| xl | 1238px | css |
| xl | 1239px | css |
| xl | 1240px | css |
| xl | 1280px | css |
| 2xl | 1284px | css |
| 2xl | 1285px | css |
| 2xl | 1348px | css |
| 2xl | 1359px | css |
| 2xl | 1360px | css |
| 2xl | 1395px | css |
| 2xl | 1396px | css |
| 2xl | 1405px | css |
| 2xl | 1406px | css |
| 2xl | 1439px | css |
| 2xl | 1440px | css |
| 2xl | 1459px | css |
| 2xl | 1460px | css |
| 2xl | 1467px | css |
| 2xl | 1468px | css |
| 2xl | 1509px | css |
| 2xl | 1510px | css |
| 2xl | 1559px | css |
| 2xl | 1560px | css |
| 2xl | 1583px | css |
| 2xl | 1584px | css |
| 2xl | 1599px | css |
| 2xl | 1600px | css |
| 2xl | 1659px | css |
| 2xl | 1660px | css |
| 2xl | 1719px | css |
| 2xl | 1720px | css |
| 2xl | 1759px | css |
| 2xl | 1760px | css |
| 2xl | 1761px | css |
| 2xl | 1762px | css |
| 2xl | 1779px | css |
| 2xl | 1780px | css |
| 2xl | 1880px | css |
| 2xl | 1920px | css |
| 2xl | 2120px | css |

**Approach:** Use `@media (min-width: ...)` queries matching the breakpoints above.


---

## 10. Agent Prompt Guide

Use these as starting points when building new UI:

### Build a Card

```
Background: #f2f2f2
Border: 1px solid #3f3f3f
Radius: 26px
Padding: 16px
Font: kakaopay System Sans
Use shadow tokens from Section 6.
```

### Build a Button

```
Primary: bg #ff385c, text white
Ghost: bg transparent, border #3f3f3f
Padding: 8px 16px
Radius: 26px
Hover: opacity 0.9 or lighter shade
Focus: ring with #ff385c
```

### Build a Page Layout

```
Background: #ffffff
Max-width: 1127px, centered
Grid: 4px base
Responsive: mobile-first, breakpoints from Section 9
```

### Build a Stats Card

```
Surface: #f2f2f2
Label: #4a4a4a (muted, 12px, uppercase)
Value: #222222 (primary, 24-32px, bold)
Status: use success/warning/danger from Section 2
```

### Build a Form

```
Input bg: #ffffff
Input border: 1px solid #3f3f3f
Focus: border-color #ff385c
Label: #4a4a4a 12px
Spacing: 16px between fields
Radius: 26px
```

### General Component

```
1. Read DESIGN.md Sections 2-6 for tokens
2. Colors: only from palette
3. Font: kakaopay System Sans, type scale from Section 3
4. Spacing: 4px grid
5. Components: match patterns from Section 4
6. Elevation: shadow tokens
```
