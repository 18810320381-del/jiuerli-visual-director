---
name: jiuerli-visual-director
description: Convert a user-provided real-world photograph into a centered unfinished Jiuerli mixed-media notebook scribble while preserving major scene structure and named focal objects. Use only when the user explicitly invokes $jiuerli-visual-director. Do not invoke implicitly for generic image editing or illustration requests.
---

# Jiuerli Visual Director

Convert one user photograph into an unfinished personal notebook scribble caught mid-process. The source controls content and major geometry, not the amount of rendered detail.

## Source contract

- Honor an explicitly requested output ratio or orientation. Otherwise preserve the source orientation. Preserve major perspective relationships, silhouette hierarchy, depth order, relative placement, scale, overlaps, and explicitly named focal objects. Keep recognition through placement and characteristic silhouette rather than exact edge tracing. Permit controlled local contour deformation while holding each major form's overall bounding area, center, orientation, depth, and overlaps in place: stretch, compress, swell, pinch, tilt, or asymmetrically bend local parts by roughly 10–25%, and exaggerate one characteristic feature when useful. Simplify or omit 25–40% of visible contour length, minor corners, window counts, repeated openings, and small attachments. Keep alignments subjective and hand-drawn rather than drafting exact vanishing points. Do not invent, relocate, merge, crop, or reconstruct major content.
- Select one or two focal forms from the user's instructions; if none are named, choose the nearest principal forms.
- Keep only those focal forms relatively legible. Omit roughly 50–65% of identifiable secondary structure and leave untouched paper running through the rest. Compress every secondary face, object, window, decoration, repeated texture, atmospheric field, and surface detail into a few incomplete directional marks and rough unresolved visual clusters. Never inventory or trace micro-detail.
- Permit two to four tiny scene-appropriate notebook doodles such as dots, an open circle, a small star, or a spiral curve in negative-space gaps. Treat them as incidental thinking marks, never new scene content.

## Scene briefing

Before generating, tell the user only what was visually distilled from the source:

- Name three to five retained scene elements.
- State the one or two focal forms and why they anchor the picture.
- State the most distinctive spatial relationship, rhythm, silhouette, or mood worth preserving.

Keep this briefing concrete and specific to the photograph. Do not discuss prompt wording, rules, tools, implementation, or internal image inputs. Do not display internal skill assets. In the final response, restate the focal choice in one concise sentence so the result remains understandable after commentary is collapsed.

## Style authority

- Always attach `assets/style-authority-bplus.png` as the second image input after the user's source photograph.
- Always attach `assets/line-authority-doodle-01.jpg` and `assets/line-authority-doodle-02.jpg` as the third and fourth image inputs.
- Assign strict roles: image 1 controls subject matter, orientation, major perspective relationships, placement, scale, depth, and overlaps; image 2 controls page composition, blank-space ratio, color sparsity, unfinishedness, and handwriting integration; images 3 and 4 control only local contour deformation, line clarity, color liveliness, and variable line thickness.
- Never copy plants, buildings, people, animals, symbols, wording, or scene layout from images 2–4 into the user's scene.
- Do not render, expose, or mention the internal style assets in user-facing updates unless the user explicitly asks about skill implementation.

## Non-negotiable visual gates

- **Page occupancy:** Fit the complete drawing island, handwriting, and tiny doodles inside the central 62–68% of page width and 55–65% of page height. Preserve a continuous untouched paper band of at least 14% on the left and right and at least 17% on the top and bottom. No subject contour, color patch, or handwriting may enter this outer margin.
- **Scene-led line color:** Select three to five clear contour colors that harmonize with the source scene, with one or two dominant colors and the rest used briefly. Choose from warm brown, rust orange, ochre yellow, fresh or grey olive, dusty teal, cobalt blue, pale sky blue, muted pink, or brick red. Allow medium saturation and clear color contrast similar to spontaneous colored doodles; do not default to blue and do not force a uniformly muted monochrome palette. Use no graphite pencil, charcoal, black-pencil underdrawing, grey sketch scaffolding, smudged shading, or monochrome pencil rendering.
- **Visible, thick, lively contours:** Make focal contours clearly readable at thumbnail size using blunt medium-to-thick colored strokes. Vary thickness abruptly within the same object: major contour strokes may be roughly 1.5–3 times thicker than minor searching lines. Alternate colors along a contour when useful. Use uneven pressure, trembling bends, offset passes, blunt starts, sudden stops, and occasional thin scratch lines. Draw secondary forms at roughly 50–70% of focal line strength with fewer broken cues; keep them clearly visible, never washed-out ghost lines.
- **Controlled naïve deformation:** Preserve each major form's overall bounding area, center, orientation, depth, and overlaps, but locally stretch, compress, swell, pinch, tilt, or asymmetrically bend contours by roughly 10–25%. Exaggerate one characteristic feature when useful. Prefer lopsided, elastic, symbol-like recognition over accurate anatomy, perfect circles, straight architectural edges, or literal tracing. Keep the subject recognizable and do not relocate or merge forms.
- **Line over hatching:** Make at least 90% of all marks contours, gestures, searching passes, writing, or tiny symbols. Keep parallel hatching, scribbled fill, and color patches below 10% of all marks. Use no more than a few short hatch accents on any focal form and none across an entire roof, wall, sky, floor, table, garment, or ground plane.
- **Sparse color:** Keep at least 70% of the drawing island as exposed paper. Use color only as small dots, short bars, thin contour accents, or a few translucent scribbles; never create a continuous colored plane.

## Verbatim B+ prompt kernel

Include this block once, verbatim, in every image-generation prompt:

> Outcome: an unfinished private travel-notebook draft caught mid-process, not a refined observational pen sketch, architectural study, clean illustration, or presentation-ready artwork. Keep the page visibly imperfect and unresolved.
>
> Page: honor the output ratio and orientation explicitly requested by the user; otherwise preserve the source orientation and use a standard page ratio. Use warm off-white, slightly cream sketchbook paper with visible fine fibers, minimal yellowing, sparse tiny black ink specks, faint eraser ghosts, and incidental dirty smudges. Fit the complete drawing island, handwriting, and tiny doodles inside the central 62–68% of page width and 55–65% of page height. Preserve a continuous untouched paper band of at least 14% on the left and right and at least 17% on the top and bottom; no subject contour, color patch, or handwriting may enter this outer margin. Let blank paper pass through and separate the drawn forms. No crop, full bleed, border, rectangular photo block, filled background field, or edge contact.
>
> Marks: select three to five clear contour colors that harmonize with the source scene, with one or two dominant colors and the rest used briefly. Choose from warm brown, rust orange, ochre yellow, fresh or grey olive, dusty teal, cobalt blue, pale sky blue, muted pink, or brick red. Allow medium saturation and clear color contrast similar to spontaneous colored doodles; do not default to blue or force a monochrome palette. Use blunt colored pencil, soft wax pencil, colored ballpoint, or dry crayon for the contours. Use no graphite pencil, charcoal, black-pencil underdrawing, grey sketch scaffolding, smudged shading, monochrome pencil rendering, or realistic value study. Draw focal contours with clear thumbnail-scale visibility using medium-to-thick colored strokes. Vary thickness abruptly within the same object: major contour strokes may be roughly 1.5–3 times thicker than minor searching lines. Alternate colors along a contour when useful. Use uneven pressure, trembling bends, offset and partially wrong passes, blunt starts, sudden stops, overshoot, open correction, and thin scratch interruptions. Preserve each major form's overall bounding area, center, orientation, depth, and overlaps, but locally stretch, compress, swell, pinch, tilt, or asymmetrically bend contours by roughly 10–25%; exaggerate one characteristic feature when useful. Prefer lopsided, elastic, symbol-like recognition over accurate anatomy, perfect circles, straight architectural edges, or literal tracing. Simplify or omit 25–40% of visible contour length, minor corners, window counts, repeated openings, and small attachments. Draw secondary forms at roughly 50–70% of focal line strength with fewer broken cues, still clearly visible but unresolved. Make at least 90% of all marks contours, gestures, searching passes, writing, or tiny symbols. Keep parallel hatching, scribbled fill, and color patches below 10% of all marks; use no more than a few short hatch accents on any focal form and never hatch across an entire roof, wall, sky, floor, table, garment, or ground plane. Omit roughly 50–65% of identifiable secondary structure. Avoid repeated texture, descriptive micro-detail, accurate architectural inventory, and dark tonal mass.
>
> Color and notes: keep at least 70% of the drawing island as exposed paper. Derive three to five line colors from the source, allowing medium saturation and distinct colored contours, but keep filled color sparse. Apply fill only as small dots, short bars, thin accents, or a few translucent scribbles with visible grain; never color or hatch an entire sky, wall, roof, table, ground, or object plane. Add only two or three very short, fragmentary, scene-appropriate English notes in irregular personal handwriting: mostly joined-up and flowing but not elegant, with mixed sizes or case, slight tremor, uneven spacing, long entry or exit strokes, and an occasional casual flourish. Let writing occupy gaps and weave through secondary routes using the same pens as the drawing. Add two to four tiny scene-appropriate thinking marks such as dots, an open circle, a small star, or a spiral curve inside the drawing island. Do not copy fixed phrases or symbols. Keep writing away from focal objects; reject polished calligraphy, typeset lettering, title, caption, logo, signature, and watermark.
>
> Reject refined life drawing, observational pencil sketch, graphite study, charcoal, grey underdrawing, accurate anatomy, undistorted photographic proportions, accurate pen or architectural rendering, rigid straight-edge geometry, clean sketch, smooth perfect contours, uniform line weight, pale washed-out linework, dense scene inventory, repeated-detail tracing, literal window or roof inventory, thin technical linework, dense parallel hatching, scribbled plane filling, dense crayon coverage, colored atmosphere fills, realistic tonal modeling, complete coloring, polished digital ink, vector or flat commercial art, photorealism, 3D, anime, cartoon, neon fill, broad fill, hard shadow, edge contact, weak margins, and automatic line cleanup.

## Fast workflow

1. Inspect the user's source photograph and identify its major structure, focal forms, and distinctive visual relationship.
2. Send the scene briefing before any generation call.
3. Compile one compact prompt in this order: strict input roles, source contract, focal forms, the verbatim kernel. Do not repeat the kernel in other words. Ensure the prompt names the selected focal forms and gives secondary forms a visibly lower completion level.
4. Use the image-generation workflow once with the source photograph as image 1, `assets/style-authority-bplus.png` as image 2, `assets/line-authority-doodle-01.jpg` as image 3, and `assets/line-authority-doodle-02.jpg` as image 4.
5. Return the generated raster and one concise sentence naming the focal choices. Do not silently create variants, self-retry, or run a second-pass review.

## Resource boundary

- Use only `assets/style-authority-bplus.png`, `assets/line-authority-doodle-01.jpg`, and `assets/line-authority-doodle-02.jpg` as the skill's internal style images. Do not use any other bundled or conversational style image unless the user explicitly replaces an authority image.
- Do not read any file in `references/`, `style/`, or `prompts/` by default. Do not inspect other files in `assets/`.
- Read `references/photo-sketch-full-text-style.md` only when the user's current message explicitly names that file or explicitly requests the full style rules.
- Read `references/regression-checklist-v2.md` only when the user's current message explicitly names that file or explicitly requests regression checking.
- A poor first result does not authorize loading a resource or retrying. Wait for the user's instruction.
