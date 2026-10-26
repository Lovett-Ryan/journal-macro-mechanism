# Style Catalog

## Shared structure and selection

All styles share 2.5D spatial structure and the [composition, annotation, and legend rules](style-guide.md). Establish science, directed relationships, exact labels, and semantic codes first; style determines how forms are modeled and rendered.

| Style ID | Name | Distinction | File |
| --- | --- | --- | --- |
| `minimal-2p5d` | Minimal Color-block 2.5D | Concise silhouettes and a few discrete face tones convey volume with almost no texture | [Guide](styles/minimal-2p5d.md) |
| `soft-gradient-2p5d` | Soft Gradient 2.5D | Broad continuous gradients model smooth matte forms with sparse surface detail | [Guide](styles/soft-gradient-2p5d.md) |
| `linework-2p5d` | Fine-line Diagram 2.5D | Fine contours, selective structural lines, and pale flat fills explain structure and thickness | [Guide](styles/linework-2p5d.md) |
| `relief-2p5d` | Relief Shading 2.5D | Slope shading and curvature reveal existing surface relief with little material grain | [Guide](styles/relief-2p5d.md) |
| `textured-2p5d` | Natural Texture 2.5D | Selective material texture, refined forms, and soft lighting explain natural interfaces and processes | [Guide](styles/textured-2p5d.md) |

Every style can serve natural, engineering, and system scenes. Do not choose by discipline alone or bind a style to a paper, image, palette, or object set. Cutaways, transparent media, stage sequences, and comparisons are composition methods, not separate styles. Independent local views are also not a new style: enable them only after main approval, inherit the selected rendering, and add supported detail. Do not reserve panels in the initial main figure.

## Distinguishing the five styles

| Style | Dominant volume cue | Treatment in a complex mechanism figure | Diagnostic distinction |
| --- | --- | --- | --- |
| Minimal Color-block | Silhouette and a few discrete planes | Group repeated objects, clear interfaces, little decoration | Dominant continuous shading indicates drift toward Soft Gradient |
| Soft Gradient | Broad continuous shading | Gentle primary modeling, quiet label regions, sparse texture | Grain/roughness defining materials indicates drift toward Natural Texture |
| Fine-line Diagram | Fine contours, structural turns, pale faces | Informative lines, low-contrast scene, distinct line roles | Volume remains readable from contours and structural lines without texture |
| Relief Shading | Slope, curvature, continuous height differences | Primary relief emphasized, secondary relief quiet, paths separate | Relief belongs to the actual object; flat objects do not grow hills |
| Natural Texture | Geometry, interfaces, selective material texture | Detail concentrated near mechanisms; quiet text/path areas | Texture identifies materials without turning the entire figure into dense realism |

Soft Gradient emphasizes smooth continuous modeling; Relief Shading emphasizes existing relief; Natural Texture additionally describes material surfaces. Words such as "soft," "dimensional," and "textured" may not uniquely identify a style. Do not silently mix styles. All preserve the full mechanism and a clear legend; surface detail density does not determine scientific information density.

## Confirm at task start

1. Read this catalog and check for a valid figure, batch, or project choice.
2. If unspecified, present every style above with its distinction in one question. A recommendation must leave the other choices available. Read options from this catalog rather than maintaining a separate stale list.
3. Preselection, recommendation, and timeout are not confirmation. Extract science while waiting; write the final generation prompt and generate only after an actual choice.
4. Briefly restate the choice, record ID and scope, and load the shared guide and selected file. Documentation maintenance does not trigger style selection.

A current name/ID/specific custom treatment, explicit reuse of a known prior figure, same-figure revision without a style change, or inclusion in an agreed batch/project counts as confirmation. Record custom treatment as a task override without asking again just to fit the catalog.

"Journal style" or "make it prettier" does not select a fixed style. Clarify only consequential ambiguity. For an explicit mixture, record the dominant method and any local secondary treatment, avoiding contradictory restrictions.

## Adapt and switch after confirmation

- Load rendering rules, complex-figure adaptation, English prompt, exclusions, and visible checks from the selected file; apply them to the current objects.
- Use the [shared prompt templates](prompt-templates.md). Keep style IDs in production records, not the artwork.
- For complex figures, establish chains, feedbacks, labels, and legend before arranging quiet label areas, informative interfaces, and routing corridors. Do not generate scenery first and squeeze in the mechanism later.
- For comparisons/switches, preserve core scientific geometry, objects, labels, endpoints, and codes. Record justified local layout changes. If a structurally matched comparison is requested, keep viewpoints and positions comparable.
- Adjust scene brightness and non-data intrinsic colors for readability, without swapping semantic classes or quantitative scales for aesthetics.
- Check that the selected dominant cue is visible. Correct rendering drift rather than deleting processes/labels or shrinking type.
- Do not apply a universal "flat, texture-free" restriction: Natural Texture retains useful texture, Relief Shading retains relief, and Soft Gradient retains continuous modeling.

## Preserve style through review and editable delivery

All styles use [skeleton review → complete figure → annotation removal → Visio annotations](review-and-visio.md). Generate science and appearance together in the complete figure. For removal, use the approved image as an actual input and preserve its style while removing only overlays to be restored natively. Do not generate another low-information background or simplify the scene into vector tracing for editability.

| Style | Protect during removal and assembly |
| --- | --- |
| Minimal Color-block | Existing forms and discrete face tones; no featureless white patches over removed text |
| Soft Gradient | Continuous shading, media overlaps, soft volume; no blur or excessive flattening as restoration |
| Fine-line Diagram | Physical contours, structural lines, interfaces; remove only explanatory paths, leaders, and frames |
| Relief Shading | Existing slope, curvature, relief hierarchy, actual channels; no changed terrain in repairs |
| Natural Texture | Informative texture and media forms; no smearing, quantized tracing, or uniform fill replacement |

Style instructions to retain labels/arrows/legends apply to complete figures and final assemblies. During removal, take only scene-rendering rules, not annotation-retention requirements. Rebuild Visio text, boxes, leaders, arrows, and legend as clear flat graphics matching the approved content and semantic codes.

## Add future styles

Add Markdown under `styles/` and register a unique ID, name, distinction, and link. Include visual intent, rendering rules, complex-figure adaptation, ready-to-use style prompt, exclusions, visible checks, and correction directions.

Describe transferable rendering rules without binding them to a paper, fixed figure, palette, facility, or layout. No main-workflow change is needed. A user may also select an explicit custom treatment for a task.
