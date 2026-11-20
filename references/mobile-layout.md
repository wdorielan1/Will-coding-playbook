# Mobile layout

Read for: phone-sized screens. Navigation, thumb reach, touch targets, spacing, safe areas, responsive behavior. Read it alongside another topic file when the screen is used on a phone.

## Rules

Bottom tab bar:

- Use 5 tabs in a bar 56–66px tall. Each tab fills its whole grid cell, so the full cell is the tap target. Cap the bar at about 440px wide and center it on wider screens.
- Icons about 21px at 1.8 stroke, labels 11px medium. Dim inactive tabs to about 60% (labels must still reach 4.5:1 contrast) and show the active tab at full strength. Use one accent color per bar, only on the active marker.
- Mark the active tab with more than color: lift its icon 3–5px (slightly larger, heavier stroke) and add a dot underneath, a glowing bump, or a floating orb.
- Slide one shared marker to the active tab (about 500 ms, springy ease such as `cubic-bezier(0.34, 1.3, 0.5, 1)`) instead of switching each tab's highlight on its own.
- Show new or unread on a tab as an 8px dot in a color that contrasts with the accent, ringed in the bar's color, at the icon's top-right corner.
- Glass bar recipe: backdrop blur 16–18px with saturate 140–160%, a 1px inner border (white at 12–55%), a brighter 1px top edge, and a soft shadow underneath.
- Check contrast against the glass, not the page behind it. In the demo, white icons on mid-brown glass measured about 4:1 (fine for icons only), and dim dark labels on cream glass about 4.4:1 (borderline; labels need 4.5:1). Use white icons only over dark or mid-tone glass, and dark icons and labels over light or warm glass.

## Tool

GlassNav: React plus a CSS module, with four styles (wave, spotlight, notch, lift). Needs `lucide-react` or your own icon components. Source: component files shared after https://www.instagram.com/p/DfMYnLZyQOE/ (author and licence unknown; the code is not kept in this repo).
