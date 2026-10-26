# Shared 2.5D Composition, Annotations, and Legends

## Shared structure

Use side faces, thickness, layers, occlusion, and necessary cutaways to convey scene depth on a flat page, then overlay flat mechanism graphics. Derive objects, connections, layout, and semantic colors from the current research. Apply the confirmed style for form, material, and lighting.

Separate scientific geometry from visual treatment. A style switch may change surfaces but not objects, relationships, directions, interfaces, or meaningful proportions. A block base is not mandatory.

## Forms and scene hierarchy

| Dimension | Shared requirement |
| --- | --- |
| Viewpoint and form | Oblique or approximately axonometric view, with recognizable side faces, thickness, and key structure; coherent directions across views |
| Interfaces and cuts | Distinct contact, layers, and media boundaries; cutaways/local views correspond to their source positions |
| Environment and repeated objects | Enough context to identify the scene; representative grouping instead of dense repetition when count has no scientific meaning |
| Materials and light | Selected style's modeling, quieter secondary regions, shadows clear of important content |
| Background and space | White or very pale; plan label, legend, and path corridors without an overall title taking space |
| Color and data | Separate intrinsic color, shape shading, and supported quantitative encoding; shadows do not imply unsupported values |

Physical boundaries say what exists and where. Paths say how it acts. Text and legend say what things and marks mean. All three layers matter, but every label does not need a leader.

## Application at each stage

- **Text-and-layout skeleton:** show layout, full text, hierarchy, paths, and legend for review; do not generate a separate text-free scene.
- **Complete figure:** after skeleton approval, generate science, rendering, and all flat explanations together. All completeness/readability rules here apply.
- **Optional local views:** generate separately only after main approval and object selection. Inherit the style and add supported detail. Do not put locators, panels, or reserved space into the initial figure. Load the separate module at the appropriate stage.
- **Clean scene:** after complete-figure approval, edit that actual image to remove text, frames, leaders, mechanism arrows, symbols, and legend while preserving physical content, natural process forms, and rendering. This intentionally incomplete intermediate asset is not the final mechanism figure.
- **Visio assembly:** retain main/local images as separate rasters and restore all explanations and source correspondences with native objects using the approved content and initial styles here. Finish after insertion and saving. Later text/box formatting belongs to the user; do not repeatedly check or adjust items or reduce style quality to simplify tracing.

See [review, removal, and Visio](review-and-visio.md) for detailed stage boundaries and scene/overlay classification.

## Labels and visual restraint

Default to no overall in-figure title, including a decorative English restatement of the paper or figure title. Put titles and sources outside, unless explicitly requested. Necessary panel letters, region names, and legend headers are allowed.

| Information | Preferred treatment | Placement and wording |
| --- | --- | --- |
| Key objects, layers, media, regions | Direct names | Inside or immediately beside the object; short words/phrases without covering interfaces |
| Locally recognizable processes | Short process name, thin frame if categorized | Beside the active region/path, without decorative leaders |
| Necessary secondary conditions | Highly transparent white-backed short note | Nearby whitespace/low-detail area, no leader, ideally one or two lines |
| Small or still-ambiguous targets | A few short leaders | Try moving text first; point accurately to one target |
| Background statistics, broad summaries, long discussion | External caption or production record | No abstract-repetition panels; design separate data graphics only when needed by the research question |

- Start white text-box fills at 60–80% transparency (20–40% opacity) and adjust for contrast. No shadows, thick borders, callout tails, or card decoration. Do not increase opacity to cover mechanisms.
- Ordinary object names are usually unboxed. Process categories may use thin outlines and nearly transparent white interiors. Pale solid fills mark drivers where needed; do not turn every label into a solid colored pill.
- Keep text and legends flat and crisp, with a conventional sans-serif or requested font and consistent hierarchy. Do not tilt them with surfaces or apply perspective/material lighting.
- Achieve simplicity through short labels, local grouping, whitespace, and scene hierarchy. Control scientific information and texture density separately; do not delete processes or shrink text for neatness.
- Complete figures and final Visio assemblies retain labels and legends. Omit explanations only for an explicit text-free request or the approved intermediate removal stage. Clean scenes also remove frames, leaders, and mechanism arrows to be restored natively; deleting words alone leaves unwanted overlays.

## Legends and semantic codes

Object names are not a legend. A legend explains colors, line styles, borders, fills, arrows, and symbols. Every actual semantic code must correspond to its legend sample and meaning.

Where the roles exist, distinguish these mark grammars. Derive category names, counts, and colors from the study rather than another subject:

| Mark grammar | Role | Legend sample |
| --- | --- | --- |
| Pale solid background | Drivers or external influence classes | Matching solid swatch |
| Thin outline or highly transparent white frame | Process class | Same-color/weight outline, not a solid swatch |
| Directed colored line | Transfer or influence pathway class | Matching line, color, style, and endpoint |
| Other symbol, range, quantitative scale | Condition, state, region, or data | Actual symbol/range style and accurate definition |

- Do not invent driver/process categories merely to fill three grammars. Simple figures use only necessary entries.
- Within one grammar, a color/line style has a stable meaning. Paths with different meanings must not share an incorrect class just because they occur in the same environment. Add a legend entry when adding a class.
- Different grammars may share a color family, but fill, outline, and arrow roles remain distinct and separately illustrated. Color names do not replace scientific definitions.
- Check legend-to-scene and scene-to-legend. Remove unused entries and explain all actual codes, including endpoints, branches, and influence symbols.
- Position the legend according to whitespace and reading order, without fixed bottom placement, column count, or area ratio. Keep its hierarchy coherent and avoid covering scenes/paths.
- Quantitative scales, widths, proportions, and contours require evidence and explanation. Schematic line weights imply no quantity.
- Preserve codes through style changes, adjusting scene brightness/contrast as needed rather than swapping category colors or changing value scales.

## Process paths, entities, and leaders

- Rivers, pipes, and physical bands are entities with necessary geometry. Abstract transfer, causality, and feedback use flat lines rather than thick 3D tubes.
- Establish source, target, meaning, and direction before choosing curvature. Branches, series, merges, and loops must match the science; see [mechanism design](mechanism-design.md).
- A crossing is not automatically a connection. Merge only connected paths; otherwise separate, interrupt, or layer them with traceable endpoints.
- Route through whitespace/corridors, clear of words, important interfaces, and other paths. Move labels or quiet scene detail rather than hiding wrong intersections with white boxes.
- Trace every path from tail to head. Avoid floating endpoints, wrong adjacent targets, or false connections through decoration. Keep independent parallel lines spaced apart.
- Distinguish object contours, hidden structures, range boundaries, process arrows, and annotation leaders. Leaders locate only and do not encode processes.
- Preserve dynamic meaning in feedback and circulation. Do not replace difficult curves with a static letter, isolated sign, or undirected circle.
- Check physical flow and causal direction separately. A flux increase/decrease does not automatically reverse movement.

## States and multiple processes

- Place core objects, the main chain, and necessary feedback first, then background. Keep local labels near their processes with a clear hierarchy.
- If opposing effects arise from different states/conditions, show distinct regions, surfaces, or comparisons rather than contradictory labels on one undifferentiated object.
- Use purposeful cutaways, state comparisons, or panels in reviews, not cards to hold long discussion.
- Distinguish historical observations, projections, committed quantities, and long-term potential. Do not invent apparently quantitative trends without time-series evidence.
- Observations or model links may have explicit visual structures when central to the figure; keep mere article background outside the mechanism scene.
- Restrained academic diagrams rely on clear interfaces, legends, short labels, paths, and hierarchy. A journal name is neither a style specification nor submission certification.

## Common drift and correction

| Problem | First correction |
| --- | --- |
| Attractive scenery but missing names/processes | Restore objects, labels, and chain from the specification; reduce decoration, not mechanisms |
| Legend samples differ from scene marks | Correct fill/outline/arrow samples and cross-check categories |
| Arrow starts at the wrong object or joins a neighboring label | Re-establish anchors and redraw that segment, preserving correct paths |
| Leader tangle or lines through words | Move labels, use whitespace, or separate layers; recheck endpoints |
| Large title or abstract-like notes consume space | Move title/long text outside; retain necessary short labels and legend |
| Selected style becomes generic realistic illustration | Restore its dominant rendering cue and reduce competing cues without losing science |
| Views disagree in appearance or information | Align style and encoding; reconcile matching objects and relationships |
