---
name: santosstudio-ui-components
description: "Create modern UI components with Santos Studio standards - bold aesthetics, 12-20px radius, 6-32px spacing, glassmorphism, and creative colors that avoid AI clichés"
---

# Santos Studio UI Components

Professional component library with bold, modern aesthetics that stand out from generic AI-generated designs.

## Philosophy

Santos Studio creates **distinctive, engaging interfaces** that avoid generic AI aesthetics:

- **Dare to be different** - Make bold creative decisions that differentiate from competitors
- **First impressions = seduction** - Onboarding and initial screens should be beautiful, not minimal
- **Context-driven effects** - Use glassmorphism, glow, and skeuomorphism when they add value
- **No AI tool clichés** - Avoid purple gradients, soft pastels, and predictable layouts

**Core belief:** Users are seduced by beauty and clarity, not by "safe" minimalism.

## When to Use This Skill

Trigger this skill when the user:
- Asks to create buttons, cards, inputs, forms, or modals
- Wants "modern", "professional", "clean", or "bold" design
- Needs help with spacing, padding, or component styling
- Mentions wanting to avoid generic or AI-generated aesthetics
- References Santos Studio design standards

## Component Recipes

### Buttons
See `buttons.md` for the complete 4-type button system:
- **Primary** (main actions, colored, gradient border on dark)
- **Secondary** (gray, less prominent)
- **Tertiary** (transparent, text-like)
- **Link** (inline, minimal)

Quick specs: 16px horizontal padding, 12px vertical, 12-16px radius, colored shadows.

### Cards
See `cards.md` for card patterns:
- **Standard cards** (white/dark background, subtle shadows)
- **Glassmorphism cards** (for premium feel on colored backgrounds)

Quick specs: 16-24px padding, 16-20px radius, backdrop-filter blur for glass effect.

### Inputs
See `inputs.md` for input field specifications:
- Generous padding (20px horizontal, 16px vertical)
- Clear states (focus, error, disabled)
- 16-20px radius

### Modals & Bottom Sheets
See `modals.md` for modal patterns:
- Desktop modals (centered, overlay)
- Mobile bottom sheets (slide up from bottom)
- Proper spacing and structure

## Design Systems

### Spacing
See `spacing.md` for the complete spacing scale.

**Quick reference:** 6, 8, 12, 16, 20, 24, 32px (extend to 40, 48, 64px for large layouts)

### Colors
See `colors.md` for color philosophy and rules.

**Quick rules:**
- ❌ **NEVER** purple as primary (AI cliché)
- ❌ **NEVER** red as primary (errors only)
- ✅ Prefer: pink+orange, blue+green, monochrome

### Signature Effects
See `effects.md` for implementation details.

**Quick effects:**
- **Glassmorphism**: backdrop-filter blur, rgba backgrounds, gradient borders
- **Glow**: colored shadows matching element
- **Skeuomorphism**: contextual (mechanical products only)

### Motion & Interactivity (CRITICAL)
See `motion.md` for complete motion guidelines.

**ALL interactive elements MUST have:**
- ✅ Hover states (scale, shadow, or background)
- ✅ Active states (pressed effect)
- ✅ Smooth transitions (150-300ms)
- ✅ Focus states (accessibility)

**Quick motion:**
- Buttons: `hover:scale-102 active:scale-98 transition-all duration-150`
- Cards: `hover:-translate-y-1 hover:shadow-xl transition-all duration-200`
- Icons: `hover:scale-110 hover:bg-gray-100 transition-all duration-150`

**Philosophy:** Components must feel ALIVE and responsive, not static.

## Quick Reference Card

```
SPACING:    6, 8, 12, 16, 20, 24, 32 (40, 48, 64 for heroes)
RADIUS:     12-16px (buttons), 16-20px (cards/inputs)
TYPOGRAPHY: 12, 14, 16, 24px | Inter default
COLORS:     No purple/red primary | Bold combos preferred
EFFECTS:    Glassmorphism (premium), Glow (tech), Skeuomorphism (contextual)
PHILOSOPHY: Dare to be different, seduce users, avoid AI clichés
```

## Motion & Interactivity (CRITICAL)

**Santos Studio components must feel ALIVE:**

### Required Interactive States

**ALL clickable elements MUST have:**
- ✅ Hover state (scale, shadow, or background change)
- ✅ Active state (pressed effect)
- ✅ Smooth transitions (150-300ms)
- ✅ Focus state (for accessibility)

**Example (button):**
```jsx
className="
  transition-all duration-150
  hover:scale-102 hover:shadow-lg
  active:scale-98
  focus:ring-3 focus:ring-blue-100
"
```

**Example (card):**
```jsx
className="
  transition-all duration-200
  hover:-translate-y-1 hover:shadow-xl
  cursor-pointer
"
```

### Motion Guidelines

**Transition durations:**
- Quick (buttons, icons): `duration-150` (150ms)
- Standard (cards, inputs): `duration-200` (200ms)
- Slow (modals, slides): `duration-300` (300ms)

**Easing:**
- Default: `ease-out` (natural deceleration)
- Exits: `ease-in` (acceleration)

**Transforms:**
- Hover scale: `scale-102` to `scale-105` (subtle enlargement)
- Hover translate: `-translate-y-1` to `-translate-y-2` (elevation)
- Active scale: `scale-98` (pressed effect)

### What Makes Components "Alive"

- Buttons grow slightly on hover
- Cards elevate on hover (if interactive)
- Icons respond to hover (background tint or scale)
- Inputs show clear focus states
- Smooth transitions on all state changes
- Immediate visual feedback on interaction

**Philosophy:** Every interaction should feel responsive and intentional. Static UIs feel dead.

## Best Practices Summary

### Do's ✅
- Use bold, saturated colors
- Make first screens beautiful (onboarding matters)
- Apply glassmorphism on colored backgrounds
- Give components generous padding
- Use 16-20px radius for cards and inputs
- Create depth with shadows and layers
- **Add hover/active states to ALL interactive elements**
- **Use smooth transitions (150-300ms) everywhere**

### Don'ts ❌
- Never purple as primary (AI cliché)
- Never red as primary (errors only)
- Don't use radius below 12px
- Don't use spacing below 6px
- Don't default to "safe" minimalism
- Don't create generic layouts
- **Never create static components without hover states**
- **Never skip transitions (feels jarring)**

## Inspiration Sources

This skill draws from world-class designs:
- **Shopify Editions**: Bold creativity, 3D elements, unexpected layouts
- **Opal**: Glassmorphism, colored glows, holographic effects, dark mode mastery
- **Airbnb**: Professional spacing, clear hierarchy, polished interactions
- **Revolut**: Glassmorphism on gradients, premium 3D elements, data visualization

---

**Remember:** Santos Studio designs stand out. Make bold choices, use creative effects when relevant, and never settle for generic AI aesthetics.

For detailed implementation, consult the specific component files referenced above.
