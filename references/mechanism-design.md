# From Source Material to Drawable Mechanisms

Use this reference for paper redraws, review overviews, or multi-process scenes. Follow the [shared guide](style-guide.md) for visual rules and the confirmed file from the [style catalog](style-catalog.md) for rendering.

## Establish the figure and evidence boundary

- With a paper, inspect candidate figures, captions, and mechanism-related text to identify the core question. Do not squeeze model comparisons, data results, and unrelated figures into one mechanism scene.
- With only an abstract, depict supported mechanisms from the supplied information. Do not infer unspecified channels, interfaces, or causality from broad conclusions. Check the paper or ask only about necessary gaps.
- An original figure used as scientific evidence may be reorganized spatially and visually. Aesthetic improvement must preserve scientific connections. Verify unclear features or discrepancies with the text rather than copying doubtful relationships.
- Record each input image's role: scientific content, visual treatment, or edit target. A visual-only input must not automatically supply objects, labels, layout, or symbols to a new subject.
- A synthesis across regions or states remains conceptual. Do not present it as a measured section at one site. Record sources, time scales, and conditions in captions or production records.

## Build the minimum drawing specification

Use the same content source for the skeleton and full prompt. Choose lists or these tables according to complexity, without repeating the paper. The skeleton also needs reviewable spatial and label associations; see [skeleton review](review-and-visio.md).

| Table | Required fields | Purpose |
| --- | --- | --- |
| Objects and annotations | Object ID/parent; object/layer/region; recognition features; label ID, exact text and nearby position; evidence | What is present, what each label identifies, and how the hierarchy works |
| Directed relationships | Path ID; source/target IDs and anchors; process meaning; physical transfer/causality/regulation; direction/conditions; evidence | What an arrow means and where it starts and ends |
| Semantic encoding | Code ID; mark type; category; color/line/endpoint; actual uses; legend text | How a mark is interpreted and rebuilt natively |

Check "central claim → visible object/process → label/legend." Rich science may require more short labels, local paths, or purposeful panels. Do not impose a fixed count of labels, objects, or arrows as a quality threshold.

## Put complete information into the figure appropriately

The full prompt constrains generation; the artwork contains what readers need to understand this figure's mechanism.

| Information | Treatment |
| --- | --- |
| Core objects, media, interfaces, processes | Visible forms and nearby short names |
| Supported transfer, causality, feedback, intervention | Paths with explicit endpoints and brief process names where necessary |
| Conditions essential to interpreting direction | Nearby short qualifiers or defined conditional symbols |
| Structures that clarify different states | Corresponding regions, state contrasts, or purposeful local views |
| Historical statistics, abstract background, model differences, extended discussion | Usually captions or production records; design explicit data graphics only if central to this figure and supported |
| Paper/figure title, attribution, method notes | Outside the artwork by default; no added overall in-figure title |

Do not delete mechanisms to reduce text, or interpret completeness as printing all background in supplemental panels. Remove long notes that merely repeat the main chain or abstract instead of adding visual information.

## Verify dynamic mechanisms and relationship types

### Establish endpoints before drawing

- Physical transfer: start at the actual source/inlet and finish at the receiving object/outlet, following the process's motion.
- Causality: connect a cause or state to its consequence. A causal path is not material transport; the presence of a substance name does not make it a pipe.
- Regulation/intervention: identify the affected process or object. Support promotion, inhibition, and conditions with evidence, and define intervention marks in the legend.
- Annotation leader: locate an object only, without implying matter, energy, or causality or using a confusing process arrowhead.

When one source has multiple outputs, branch independently from that source. Do not connect adjacent labels into a production chain unless conversion is supported. Shared segments need a common source and meaning; a visual merger must not imply a nonexistent conversion.

### Validate every feedback edge

Write each critical loop as A → B, B → C, C → A and compare every edge with the actual figure. A closed shape, signs, or the word "feedback" do not establish correctness.

Spatial circulation also needs viewpoint and rotation. Letters, abbreviations, and icons may name states or objects, but cannot replace the circulation, transport, or dynamic feedback being explained. Fix endpoints, routing, or composition when arrows fail; do not remove the dynamics for neatness.

### Separate different states

- Opposing effects may arise from different surfaces, media, regions, stages, or boundary conditions. Make those distinctions visible instead of applying contradictory labels to one undifferentiated object.
- An increase/decrease is not a reversal of physical flow. Distinguish magnitude wording or supported magnitude encoding from motion arrows.
- When direction depends on conditions, use short qualifiers, branches, or defined symbols such as ±. Explain symbols in the legend; do not impose one sign on all cases.
- Without quantitative evidence, do not draw apparently dimensional arrow widths, curves, elevations, or temporal trends.

## From design to verification

Before generation, reconcile labels, directed relationships, and encoding, and show the skeleton for user review. After approval, use all necessary science and layout information to generate the complete figure. Do not separately generate a skeleton and a text-free reference scene, or omit all labels/arrows for future editing convenience.

Check the actual generated image, not merely whether a requirement appeared in the prompt. Order: objects/evidence → endpoints/directions → feedback/state distinctions → legend → text/path clearance → selected style cues. Use [targeted correction templates](prompt-templates.md) and record the executed edit chain.

For editable delivery, obtain complete-figure approval, temporarily remove overlays through [annotation removal and Visio assembly](review-and-visio.md), restore all annotations natively, and save. Then finish. Content completeness applies to the final assembly; later text, frame, and annotation formatting belongs to the user, without repeated item-level checks. The intermediate clean scene need not explain mechanisms whose overlays were intentionally removed. Do not generate images for documentation-only or feedback-recording requests.
