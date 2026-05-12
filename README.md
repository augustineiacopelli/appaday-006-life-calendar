# 006 · Life Calendar

**AppADay · Day 6 · Category: Data Visualization**  
*Built by Augustine Iacopelli · May 12, 2026*

---

## What It Does

Enter your birthdate and a life expectancy. Life Calendar renders every week of 
your life as a single mark — gold for weeks lived, red for the week you are in 
right now, dark for the weeks still ahead.

Two visualizations are available:

**Week Grid** — Your entire life laid out row by row, one row per year, 52 marks 
per row. Each year is labeled with the calendar year and your age at the time. 
Scroll from birth to the end of your expected life in a single continuous view.

**Year Arcs** — A concentric ring diagram where each ring represents one year of 
life. Rings fill clockwise from 12 o'clock. Fully lived years are solid gold. 
Your current year shows a gold arc for completed weeks followed by a red sliver 
marking the present moment. Future years sit as dark empty tracks. Your age in 
years is displayed at the center.

Add named life events — a wedding, a birth, a graduation, a move — and they 
appear as blue markers pinned to the exact week across both views, with name and 
date in the tooltip.

---

## How to Use

1. Enter your date of birth
2. Set your life expectancy (default 80 years)
3. Click **Render My Life**
4. Switch between Week Grid and Year Arcs using the tabs
5. Open the **Life Events** panel to add named dates — each one is pinned to its 
   week across both views

---

## Technical Notes

- Pure HTML, CSS, and vanilla JavaScript — no frameworks, no dependencies
- Week indexing is anchored to calendar birthdays rather than multiplying by 52, 
  which correctly accounts for leap year accumulation over a lifetime
- Year Arcs are drawn as SVG path elements using polar coordinate math — no 
  stroke-dasharray tricks
- All date parsing uses local time construction to avoid UTC offset errors

---

## Definition of Complete ✓

- [x] Functional — renders correctly on both views with accurate week counts
- [x] Single purpose — one job: visualize a human life in time
- [x] Mobile friendly — responsive at 375px viewport
- [x] Visually polished — Cormorant Garamond serif, dark contemplative palette
- [x] Published — live at GitHub Pages before midnight CDT

---

## Future Improvements

- Add export or print function to save completed calendars
- Add social buttons to send to social media
- Add additional visualizationt types
*Part of the AppADay project — one complete web application shipped every day.*  
*[← Back to Portfolio](../index.html)*
