# Skeleton Review, Annotation Removal, and Visio Assembly

For a new design, read the skeleton and review sections. Continue to the later sections for editable delivery. [Mechanism design](mechanism-design.md), the [shared guide](style-guide.md), and the selected style still govern the science and visual treatment. Use the [prompt templates](prompt-templates.md) for generation and removal.

## One continuous design chain

Text-and-layout skeleton → user review → complete mechanism figure → user review → derive a clean scene from that figure → native Visio annotation assembly.

For local views, add "confirm detail subjects → separately generate the clean main and independent local images" after main approval. Before then, do not load the local module or put its requirements, example images, or reserved layout into the initial call. Once the user opts in and approves the main figure, read the [local detail module](local-detail-views.md) and select subjects. Do not generate any branch asset before main approval.

The skeleton supports design review. The complete figure coordinates scene, materials, text, and mechanisms together. Derive the clean scene only from that approved complete figure. Do not independently generate a skeleton and text-free reference scene and then try to reconcile their content/positions by collage. The clean scene is an intermediate assembly asset, not a reduced final mechanism figure.

Retain the selected shading, texture, media forms, and necessary detail as a raster. Visio makes all flat explanations editable. Do not rebuild trees, mountains, or smoke as native vectors or route through Illustrator, tracing, or whole-scene SVG. No OCR service or token is needed.

## Skeleton: make the planned figure reviewable

Default to a readable Markdown design containing spatial notation and inventories. Complex layouts may include a simple wireframe of regions, words, and paths. No image generator is needed; do not use the wireframe as the complete figure's material/style reference.

| Content | Record at least |
| --- | --- |
| Figure settings | Style ID/override, frame, language, font, no-overall-title convention, scientific scope |
| Spatial layout | Viewpoint, front/back/left/right regions, required cutaway/view correspondence, label corridors, legend area |
| Object hierarchy | Region → object → meaningful element; object/parent IDs, recognition features, scientific reasons for grouping or subdivision |
| All text | Label ID, exact wording, type, associated object/process, nearby position, frame style, type hierarchy; all legend headings and symbol definitions |
| Leaders and paths | ID, source/target or label target, meaning/condition, color/line/endpoint, clear route and avoidance requirements |
| Legend | Code ID, exact term/sample, and actual objects/paths using it |

Put labels back into space through a text layout or position table; a word list is insufficient. "Place L1 in the whitespace above-right of object A1 in region A" is more reviewable than "L1 goes top-right." Keep boxes near their object or active region instead of pulling all text to the perimeter for tidy alignment.

Hierarchy is semantic: an object may comprise related elements or be a named geographic region. Record the granularity needed for mechanism understanding and later annotation. Repeated objects may form a region; individual tree/leaf decomposition is unnecessary.

For precise assembly, record canvas `W × H`, a top-left origin with positive right/down, and normalized coordinates `u=x/W, v=y/H`; boxes use `[u,v,w/W,h/H]`. Skeleton coordinates constrain regions and adjacency. Calibrate final positions against the actual complete and clean images.

Classify scene and overlays separately. Physical contours, rivers, natural plumes, precipitation forms, and material interfaces belong to the scene. Labels, boxes, legends, leaders, causal/flux arrows, and explanatory symbols belong to editable annotations. Decide ambiguous radiation lines, circulation marks, and range boundaries by scientific role, not color or curvature alone.

## The two reviews

1. **Skeleton review:** show layout and full inventories; ask the user to check science, hierarchy, words, positions, and relationships. Wait for actual approval before generating the full figure. Revise the relevant version on feedback without generating another background.
2. **Complete-figure review:** first internally check science, labels, legend, rendering, and readability; then show the complete figure. Freeze the user's approved version as the basis for removal and assembly.

Offer useful local views at this stage. If already requested, record opt-in without asking again. Confirm subjects and external layout after main approval rather than preplacing them in the initial figure.

Style selection is not skeleton approval. Vague praise does not approve an unseen version. Reuse a clearly approved skeleton/figure at its stage; otherwise do not skip review unless the user explicitly changes the requirement. Prepare independent material while waiting, but do not execute dependent generation or assembly.

## Complete figure: generate science and appearance together

Expand all reviewed science, hierarchy, exact labels, nearby positions, relations, legend, and original research explanation in one full prompt. "Follow the skeleton" or a low-information layout image is insufficient.

The complete figure contains the chosen scene rendering plus object names, process labels, boxes, essential leaders, arrows, and legend, so it is readable by itself. Allow justified local whitespace adjustments without changing science, omitting elements, or swapping classes. Do not merge the skeleton preview and artwork as a required tool input. State the role of any actual image input.

After approval, update the annotation inventory from the actual image: object anchors, box bounds, line breaks, colors, type hierarchy, arrow routes, and legend position. Preserve scientifically correct exact text. Correct erroneous wording and confirm the affected version first; do not treat a transcription error as new evidence.

## Removal requires the actual approved image

Use reference-guided editing with the approved figure supplied as the edit target. Mentioning its filename in text is insufficient. Do not reimagine a clean scene from the abstract. Keep the approved original unchanged.

Remove and later rebuild:

- Every visible character: object/process names, panel letters, conditions, subscripts/superscripts, units, and legend headings. Unnecessary overall titles should already be absent.
- Label backgrounds, colored driver marks, process outlines, note boxes, leaders, and endpoint marks.
- Entire mechanism-arrow shafts and heads, feedback curves, annotation-only boundaries, standalone signs, and other inventoried explanatory symbols.
- The whole legend: text, swatches, outlines, arrow samples, dividers, and enclosing frames.

Distinguish label backings from actual scientific region coloring; retain the latter. Preserve all physical elements and natural process forms. Reconstruct covered scenery rather than applying white patches. Existing blank legend space may remain empty for native assembly.

| Check | Requirement |
| --- | --- |
| Scene fidelity | Compare viewpoint, frame, adjacent objects, interfaces, cuts, material states, and style, especially areas previously hidden by labels |
| Overlay removal | Inspect for residual/pseudo-text, frames, short strokes, arrowheads, legend marks, and patches; do not conceal residues later under overlays |
| Position consistency | Compare distributed physical anchors; calibrate uniform scale/translation, but repair inconsistent deformation or moved objects |
| Resolution | Record actual output size and preserve aspect ratio; do not claim upscaling restores detail or deliberately lower image quality for alignment |

Generative differences are possible; pixel identity is not guaranteed. Repair significant object/material changes before assembly. Do not force old coordinates onto a changed scene or claim unverified fidelity. The approved figure remains the quality baseline.

## Visio: layered scene and annotations

Use an available Visio connector or Windows application control. Programmatic native-file authoring is also allowed. Perform one overall confirmation that the file is usable and scenes/annotations display; a current Visio view or user confirmation suffices. Do not reopen or run edit/undo trials repeatedly. Record actual missing-tool/runtime limitations without reverting to tracing or claiming an incomplete/unusable file is finished.

Suggested layers, named for the study as appropriate:

| Layer | Content and editing requirements |
| --- | --- |
| Main scene | Embed the clean image, preserve aspect ratio, place at bottom and lock; avoid broken external links |
| Local views, when enabled | Independently embed each image, normally outside the main figure on an expanded page; never preflatten with the main image |
| Mechanism paths | Native lines/curves/connectors and endpoints retaining color, style, width, and direction |
| Leaders | Native locator lines, distinct from mechanisms |
| Source correspondence, when enabled | Native locator circles/range frames and a few no-arrow dashed lines; identify main/detail correspondence only |
| Text and frames | Native text, adjustable fills/transparency, editable borders; ordinary object names can remain unboxed |
| Legend | Native words, swatches, process outlines, arrows, and condition symbols; reasonable groups with individual editing inside |

Restore all explanations from the approved figure and calibrated clean image, including secondary object names, units, conditions, and legend. Text outlines, SVG text paths, or legend screenshots are not editable text. Do not flatten the annotation layer.

For a clean-image origin `(x0,y0)` and displayed size `(Bw,Bh)`, top-left coordinates map to `x=x0+u*Bw, y=y0+v*Bh`. With a bottom-left interface, points use `y=y0+(1-v)*Bh` and box bottoms use `y=y0+(1-v-h)*Bh`, where `h` is normalized box height. Use actual dimensions and interface conventions; do not mix pixels, points, and page units.

Associate annotations with object IDs through names/custom data. Raster scene regions may have recorded anchors without pretending to be native connectable objects. Place paths by scientific endpoints. Groups should move together while allowing individual text/frame/line edits. Set initial styles from the approved figure and [shared guide](style-guide.md), without opaque cards hiding removal residues. Do not start an item-by-item formatting loop afterward.

## Completion and delivery

- **Completion point:** independently embed the clean main and all selected local images, add all text, boxes, required leaders, mechanism arrows, source locators, and legend natively at their positions, and save a usable Visio file.
- One overall confirmation is sufficient: scenes/explanations display, content is restored, and annotation objects are editable. Use a current app view or user confirmation; do not try-edit/restore every word, drag/undo arrows, test legend members, or repeatedly save/reopen.
- **Formatting belongs to the user:** after initial assembly, do not default to checking/refining font details, sizes, wrapping, character spacing, box dimensions, opacity, border weights, spacing, alignment, or tiny position differences. Do not delay delivery because these could improve. Refine on an explicit follow-up request.
- Missing content, flattened text, corruption, or absent scenes mean assembly is unfinished and need repair. Science was established during skeleton/full-figure review; do not rewrite it as final formatting.
- Deliver native Visio and retain skeleton, approved figure, clean assets, annotation manifest, and actual prompt chain. A preview is optional when requested or already available, not a mandatory final export. Identify the raster scenes and native editable annotations accurately.
- Record truthful states: `skeleton awaiting review / skeleton approved / figure awaiting review / figure approved / clean scene needs repair / assembling Visio / workflow complete`. Later user formatting is not unfinished work. Documentation-only updates are not executed figure tests.
