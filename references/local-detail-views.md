# Local Detail Views After Main-Figure Approval

Load this module only after the annotated main figure is approved and the user has enabled local views. It does not participate in initial main-figure prompting. An advance request enables the later branch but does not bypass main review or object selection.

## Capability and scope

A "micro view" here enlarges a macro object's local structure, interface, or physical process to reveal principles unclear in the overview. Additional detail needs evidence. Exclusions for cells, molecular biochemistry, and electronic-device mechanisms remain. Do not invent material structure, scales, magnification, porosity, or other quantitative information.

Inherit the confirmed main style, object identity, colors, light direction, material states, and structural connections. Do not introduce a generic separate "micro style." Increase geometry and surface detail only when informative, without switching to another highlight/material/realism treatment. Preserve each style's dominant modeling cues.

## Confirm subjects and layout

After main approval, propose useful candidates with reasons if subjects are not yet selected. Let the user choose rather than automatically generating a fixed count. Reuse already specified objects and explanations without asking again.

Record a concise specification per subject:

| Field | Content |
| --- | --- |
| Local-view ID | Independent asset name and associated main-figure version |
| Source object | Main object ID, region, recognizable anchor/range |
| Explanatory focus | Structures, interfaces, states, processes, and evidence boundary |
| Physical forms | Required elements/connections, distinguishing entities from explanatory overlays |
| Later annotations | Exact short labels, necessary paths/symbols, saved in the native assembly inventory |
| Image inputs | Approved main, relevant region image if available, necessary scientific/visual material and each role |
| Assembly | External position, displayed size, source locator, correspondence route |

Default to an expanded page with details outside the main figure, preserving its composition, aspect ratio, and required content. Arrange details in reading order, subordinate to the overview. Size/count follow explanatory need; do not shrink the overview into a thumbnail. Follow any user-specific layout.

Use thin source locators and, when needed, a few no-arrow dashed correspondence lines. They indicate correspondence only, not causality, flux, or movement, and must differ from mechanism paths. Avoid words, important objects, and legends; do not create a leader network. A rectangular range is allowed when useful, without implying a physical boundary.

Later examples supply only the presentation of enlargement/correspondence. Do not import their discipline, objects, labels, palette, clipping defects, or fixed layout.

## Generate independent assets and isolate inputs

After specification confirmation, separately generate the clean main and each local image, saving independent files. Use the [shared removal template](prompt-templates.md) for the approved main. A simple enlarged low-resolution crop is not new local detail.

Each local call receives only its full specification, necessary science, actual reference images, and confirmed rendering rules. Keep different subjects in separate calls; exclude unrelated local-view elements, labels, and layouts. Select explicit image paths rather than automatically including recent conversation images.

Inspect every main/local input, stating which supplies identity/position, material, or science. Do not invent unsupported internal processes. Ask or verify sources when a gap affects correctness.

### Independent local-view prompt

```text
Use case: scientific-educational.
Asset: one standalone, annotation-free close view of a specified object from the supplied approved scientific scene.
Input roles: {actual supplied approved scene -> object identity, palette and rendering; supplied local region -> location and geometry; any scientific reference -> only the supported structure}.
Subject: {one selected object and the exact local structure/interface/process to reveal}.
Scientific basis and limits: {supported features, states and relationships; uncertainties and details not established by the sources}.
Required physical elements: {recognizable shapes, interfaces, physical pathways and state differences}.
Composition: {local viewpoint and framing; the complete relevant object/structure remains readable}.
Rendering: {confirmed style's volume cues, palette, light direction and material treatment taken from the approved scene}; increase only the informative local detail while keeping the same visual language.
Preserve {object identity, meaningful boundaries, topology and state}. Keep physical features distinct from explanatory graphics.
Output one complete independent image of this subject, {aspect ratio, dimensions and background appropriate to the selected object}. No text, label boxes, explanatory arrows, legend, locator marks, title, watermark or surrounding page layout. These overlays are kept in a separate authoring specification.
Do not invent quantitative scales, magnification ratios, internal structures or additional mechanisms. Do not include unrelated objects or other selected subjects.
```

Save every actual full prompt, image-input list with roles, output path, and dimensions. Check object, interfaces, states, and explanatory content against the main figure and ensure no text/arrows remain. Pixel identity is unnecessary.

## Visio assembly and completion

- Independently embed the main and each detail image so they can be selected, moved, and scaled separately. Never preflatten them into one large raster.
- Add native ellipses/ranges, no-arrow correspondence lines, text boxes, process arrows, and legend samples. Keep short labels near actual structures. Reuse main semantic codes; explain any necessary new code.
- Keep scene/detail content as rasters and explanations as editable native objects. Do not burn locators, borders, or legends into images.
- Once the main, all selected details, and their annotations are positioned, saved in a usable Visio file, and confirmed in one overall view, finish. Later type sizes, box dimensions, transparency, alignment, and tiny position adjustments belong to the user. No item-level polish loop or mandatory preview export.
- Without main approval or subject confirmation, remain at the corresponding review stage rather than generating assets early to force completion.
