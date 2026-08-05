---
name: translate-presentation-faithfully
description: Translate an existing PowerPoint, Google Slides, Keynote-exported PPTX, or presentation PDF while preserving the source deck's design, structure, product identity, facts, figures, tables, charts, images, logos, and slide order. Use for literal or publication-ready presentation translation, especially technical manufacturer decks, product catalogs, commercial materials, and requests such as “translate only”, “do not redesign”, or “keep everything unchanged”.
---

# Translate a presentation faithfully

Treat this as controlled document localization, not presentation design.

## Establish the contract

Confirm or infer the source and target languages. Work on a copy and preserve the source.

Apply this priority order:

1. Preserve facts, product identity, model names, numbers, units, formulas, certifications, warnings, and legal meaning.
2. Preserve slide order, masters, layouts, objects, images, charts, tables, logos, colors, typography, and visual hierarchy.
3. Produce correct, natural target-language copy that fits the inherited text containers.

Do not rewrite marketing claims, improve the offer, add explanations, replace images, modernize the design, or correct a suspected source error silently.

## Inspect before translating

Inspect every slide, notes page, master/layout, chart label, table cell, grouped shape, and image containing text. Create an inventory of translatable and protected content.

Classify strings as:

- translate;
- keep verbatim;
- transliterate only if the target market requires it;
- verify because the source is ambiguous or apparently inconsistent.

Read [references/translation-rules.md](references/translation-rules.md) for terminology, numbers, units, warnings, charts, tables, and image text.

## Translate with a terminology lock

Build a glossary before bulk replacement. Lock manufacturer names, trademarks, model codes, protocols, electrical abbreviations, units, and repeated feature names. Use one translation for one concept throughout the deck.

Translate meaning precisely. Keep sentence length close to the source where possible. Shorten by removing linguistic redundancy, never by dropping a technical condition or commercial limitation.

If source text is unclear, preserve it and flag it instead of inventing an interpretation.

## Edit inherited elements only

Use the platform's native presentation-editing capability. Preserve the source master-layout-slide hierarchy and edit existing text-bearing elements in place.

Never rebuild the deck from screenshots or visual imitation when an editable source exists. Never flatten editable content unless the user explicitly requests a static output.

If text does not fit, try in this order:

1. choose a shorter faithful translation;
2. adjust line breaks inside the same box;
3. use an approved source-layout alternative only if the user allows layout changes;
4. report the affected slide as blocked.

Do not silently shrink fonts, move objects, resize equipment images, or change the composition.

## Run semantic and visual QA

Read [references/qa-checklist.md](references/qa-checklist.md). Render and inspect every final slide at full size. Check translated text against the source slide by slide, then check the exported editable file itself.

Deliver the translated copy and a concise exception log only when ambiguities or unavoidable fit issues remain. Do not burden the user with routine process notes.
