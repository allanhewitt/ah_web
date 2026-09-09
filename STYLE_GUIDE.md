# AH Web Style v1

This repository uses a shared visual language for simple public one-off webpages.

## Purpose

The house style should feel clear, restrained and deliberately designed. It is intended for teaching pages, project summaries, explainers, diagrams and similar lightweight public resources. It should not feel like a generic template, a dashboard, or a heavily branded marketing site.

## Core principles

- Prioritise readability and hierarchy over decoration.
- Keep the reading column narrow enough for comfortable prose.
- Use generous vertical spacing and visible section rhythm.
- Use one dark structural colour, one mid-tone blue and one restrained accent colour.
- Prefer simple dividers, subtle callouts and lightweight tables over cards and heavy UI chrome.
- Avoid unnecessary icons, gradients, shadows and decorative effects.
- Let the content determine the page structure. Do not force every page into identical components.
- Maintain responsive behaviour for phones and narrow screens.
- Avoid em dashes in published prose. Use commas, colons, semicolons or parentheses where appropriate.

## Typography

- Headings: Source Serif 4, with Georgia as fallback.
- Body text: Inter, with system sans-serif fallback.
- Main title: large serif, strong but not oversized.
- Section headings: serif, medium weight, dark navy.
- Body copy: compact but comfortable, around 1.55 line-height.
- Small labels and metadata: sans-serif, restrained size and colour.

## Colour palette

The canonical values are defined in `assets/ah-web.css`.

- Navy dark: `#16324a`
- Navy: `#1f4e79`
- Navy mid: `#3a6b96`
- Light tint: `#eaf1f7`
- Paper background: `#fbfaf6`
- Main ink: `#24303a`
- Slate text: `#5b6a75`
- Amber accent: `#b9722c`
- Divider line: `#d7e1e8`

## Layout

- Main content width: approximately 760px.
- Page gutters: 24px on standard screens.
- Large vertical spacing between major sections.
- Masthead spans the viewport width while its content aligns to the main reading column.
- Footer aligns to the same reading width as the page body.

## Reusable components

The shared stylesheet currently provides:

- `.masthead` and `.masthead-inner`
- `.kicker`
- `.lede`
- `.wrap`
- `.lead-list`
- `.callout`
- `.timeline`, `.tl-item`, `.tl-dot`, `.tl-date`, `.tl-title`, `.tl-desc`
- `.steps`, `.step`, `.num`
- `table.assess`
- shared footer styling

Use only the components that suit the page. A short image-led explainer may need only a masthead, image, caption and a few sections.

## Images and figures

- Use clear, high-resolution images with meaningful alt text.
- Keep figures within the reading width unless there is a strong reason to extend beyond it.
- Prefer captions in muted slate text.
- Avoid stock-like decorative imagery when the page is primarily explanatory.

## Accessibility

- Preserve semantic HTML: headings in order, real lists, real tables and meaningful link text.
- Provide alt text for informative images.
- Keep sufficient colour contrast.
- Do not use colour alone to communicate meaning.
- Ensure layouts collapse cleanly on narrow screens.

## Page-specific CSS

New pages should normally load the shared stylesheet:

```html
<link rel="stylesheet" href="../assets/ah-web.css">
```

A page may add a small local `<style>` block after the shared stylesheet when its content needs a unique component. Do not modify the shared stylesheet for a one-off exception unless the change should apply to future pages as well.

## Canonical starting point

Use `templates/standard-page.html` as the normal starting structure for a new page.

The B1408 guide at `b1408-guide/index.html` is the original reference implementation from which AH Web Style v1 was derived.
