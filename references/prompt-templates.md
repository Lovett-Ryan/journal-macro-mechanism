# Prompt Templates and Targeted Corrections

## Usage

Confirm the style through the [catalog](style-catalog.md), then read the [shared guide](style-guide.md) and selected style. Establish coverage, relationships, and codes with [mechanism design](mechanism-design.md); submit the [skeleton](review-and-visio.md). Write the complete-figure prompt after skeleton approval. Use the removal template and assemble Visio only after complete-figure approval.

Replace braced fields and remove inapplicable lines; do not submit an unchanged template. Insert the selected style prompt and exclusions once. Translate its complex-figure adaptation into concrete treatment of this scene. Keep style IDs, sources, and figure names in records rather than printing them by default.

## Current-stage input boundary

The initial prompt includes only current main-figure science, approved skeleton, labels, codes, and style. Rebuild the full prompt explicitly rather than copying the conversation, historical edit chain, or future plans. Future local subjects, locators, correspondence lines, reserved positions, and layout examples do not enter this call, even as negative instructions. Retain the main scene's own required cuts/layers.

Save the actual stage prompt and image-input list, and submit only listed images. Later local-view examples are excluded from initial generation. Load local prompts from their separate module only after main approval and opt-in; do not add them to this initial template.

## Skeleton review draft

This is a user-facing design, not a prompt for a text-free scene. Use text layouts, position tables, or simple wireframes according to complexity, without generating another reference image.

```text
Skeleton version: {version}; confirmed style and scope: {style / scope}.
Frame/language/font: {settings}; core question and evidence boundary: {scope}.
Spatial layout: {viewpoint; front/back and left/right regions; cutaway; label corridors; legend area}.
Object hierarchy: {region ID -> object ID -> meaningful element ID; parent; recognition feature}.
Labels and boxes: {label ID -> exact text -> object/process ID -> nearby position -> text/box style}.
Paths and leaders: {ID -> source/target anchors or annotation target -> meaning/condition -> routing and mark}.
Legend: {code ID -> exact term and native sample style -> actual uses}.
External information: {caption, source and necessary extended explanation}.
Open questions: {only unresolved scientific or layout decisions}.
Review request: Please check this version's content, hierarchy, label positions, and connections. After approval, generate the complete mechanism figure from this design.
```

## After skeleton approval: complete mechanism figure

```text
Use case: scientific-educational.
Asset: an annotated scientific journal macro-scene mechanism figure.
Primary request: Explain {central mechanism and scope of this figure}.
Approved design specification: {the actual reviewed skeleton version; expand all its scientific content, hierarchy, spatial and annotation requirements below}.
Create one complete, coherent figure integrating the scene, selected surface treatment, all required labels, frames, essential leaders, mechanism arrows and legend. Do not generate a background-only reference, rasterize a wireframe as the final visual, or paste a text skeleton over a separately generated scene.

Input roles, if any:
- {image -> scientific content, visual treatment, or edit target; explicitly state which aspects may be reused}.
Scientific basis: {relevant supplied text, figure/caption and mechanism section; distinguish evidence from assumptions}.
Do not copy unrelated objects, symbols, layout or palettes from a visual-only input.

Scientific specification:
- Required objects and layers: {recognizable geometry, location, interfaces and meaningful scale}.
- Required processes: {main chain, supported branches, controls, outcomes and feedbacks}.
- Directed relation map: {source -> target; meaning; physical transfer / causality / intervention; direction and applicable condition}.
- Ordered feedback edges: {each edge separately; for spatial circulation include viewpoint and rotation}.
- Contrasting states: {distinct surfaces, regions or stages that produce different effects}.
- Coverage: {central claim -> visible object/process -> exact short label or legend item}.
- Evidence limits: {unsupported mechanisms/values to omit; concise conditions needed to avoid a misleading universal claim}.
Keep parallel outputs independent unless a conversion between them is supported. Do not replace a required dynamic process with a static symbol.

Composition:
{Viewpoint; foreground/background; primary objects and visible sides; necessary scene cut faces and state contrasts with clear correspondence.}
Use a coherent 2.5D scene and reserve actual whitespace corridors for labels and paths. Simplify decorative repetition rather than scientific content. Multiple views are used only when they clarify the mechanism.
No overall title inside the figure. Use {only necessary panel letters, region names and legend headers}. Keep the figure title, source attribution and background discussion outside the artwork.

Style:
{Rendering paragraph from the selected style file, adapted to the current objects.}
Style adaptation for this scene:
{How the chosen volume cues, detail distribution and treatment of repeated objects/media apply here; identify quiet label regions and informative interface regions.}
Do not mix in another style's exclusions or flatten the distinctive rendering cue of this style.

Semantic code and legend:
- Driver marks, if applicable: {category -> pale solid background -> exact legend term}.
- Process marks, if classification is useful: {category -> thin outline with nearly transparent white interior -> exact legend term}.
- Pathway marks: {meaning -> color, line style and endpoint -> exact legend term}.
- Other symbols/areas/scales, if applicable: {mark -> supported meaning and exact legend term}.
Each scene mark and legend sample must match in fill, outline, line style, color and arrowhead. Every legend entry must be used; every semantic code must be explained. Use only the categories needed for this study, not a fixed topic palette or a mandatory number of columns.
Ordinary object names are unboxed. Do not turn process outlines into solid driver-like pills. Keep physical contours, causal lines, transfer arrows and annotation leaders distinct.

Text, verbatim:
{Complete required object names, process phrases, conditions and legend terms.}
Typography: {requested language/typeface; otherwise clear conventional sans-serif; consistent hierarchy and legible size}.
Direct label placement: {exact text -> exact object/layer/process and nearby open position}.
Secondary notes, only if essential: {short phrase -> local low-detail position}. Highly transparent white background, initially 60–80% transparency, no shadow and no leader. No abstract/statistical/projection paragraphs or explanatory dashboard cards.
Essential leaders only: {ambiguous small target -> short accurate leader; omit if none}.
Caption-only information, not to render: {title, source and any necessary extended explanation}.

Path routing:
{Identify source and target anchors using distinctive geometry and location, then describe clear routes.}
Preserve actual sources, destinations and direction. Route through open space, clear of words and interfaces. A crossing is not a junction. Keep independent emissions/outputs separate and traceable. Use brief local causal returns where possible; longer feedback paths remain explicit. No orphan arrowheads, meaningless duplicate lines or false serial connections.
Physical motion direction is distinct from an increase/decrease in magnitude; encode these separately.

Output: {framing, dimensions/aspect ratio and background; white or very pale if unspecified}.
Style-specific exclusions: {only those from the selected style, plus explicit user overrides}.
General constraints: Full supported mechanism and legible labels/legend, without invented data or processes, overlapping words or obscured endpoints. No overall title, logos or watermark unless explicitly requested.
```

If the user explicitly requests an in-figure title, replace the no-title instruction with exact wording. Respect skeleton regions/adjacency, allowing small whitespace adjustments for aesthetics. Return to design review for major layout/scientific changes. Check and show the complete figure, then wait for approval of that version. Do not perform downstream generation at this stage. For enabled local views, confirm subjects after approval and then load their module.

## After figure approval: remove all overlays from the actual image

Supply the approved complete figure as the actual image input, inspect it, and identify it as the edit target. Preserve its original. Do not append complete-figure instructions or style clauses that retain all labels/arrows/legends; use only scene-rendering and fidelity requirements here.

```text
Use case: precise-object-edit.
Asset: an annotation-free raster scene derived from the supplied approved scientific mechanism figure, for later native annotation in Visio.
Primary edit target: {the actual supplied approved full figure; version and file recorded outside the artwork}.
Use this image as the visual and spatial source. Do not create a new scene from a description or redesign its composition.

Preserve:
- {viewpoint, full frame/aspect ratio, positions and silhouettes of all required objects, material regions, interfaces and cutaway geometry}.
- {confirmed style's actual volume cues, shading, selective texture and visible natural process forms}.
- Physical features and scene content: {explicit preserved entities, e.g. actual channels, natural plume shapes or material boundaries relevant to this figure}.
- {landmarks used later for label and pathway alignment}.

Remove completely:
- Every text character, label, unit, subscript, panel letter and legend heading.
- All annotation boxes and their fills/borders, leader lines and endpoint marks.
- All explanatory mechanism arrows, including their entire shafts and heads, feedback curves, annotation-only boundaries and standalone explanatory symbols: {explicit inventory or regions}.
- The entire legend, including text, swatches, outline samples, arrow samples, separators and outer frame.
Do not remove real physical contours or material regions just because they resemble an annotation line or fill. Use {the scene-versus-overlay inventory} to distinguish them.

Reconstruct the underlying scene plausibly and continuously wherever annotations hid it. Match adjacent surfaces, interfaces, lighting and texture. Keep existing quiet space for later labels and legend. Do not move, add, remove or change scientific objects or states.
No residual letters, pseudo-text, frame fragments, arrowheads, ghost lines, legend marks, white patch covers or smeared repairs. Add no replacement labels, arrows, title, logo or watermark.
Output: the complete preserved scene as a raster image, same framing and aspect ratio, at {required actual output dimensions where supported}; retain the quality and distinctive rendering cues of the approved source.
```

Inspect the result, calibrate coordinates, and restore all explanations through [Visio assembly](review-and-visio.md). Finish after native insertion and saving. Leave format refinement to the user without continued item-level text/frame checks or mandatory preview export. Deleting words while retaining mechanism arrows or legend swatches creates duplicates and is unacceptable. For a separate explicit text-free request, honor that scope without claiming this intermediate scene is a complete mechanism figure.

## Edit an existing figure

```text
Use case: {precise-object-edit or style-transfer}.
Input roles: {each target/supporting image and its allowed use}.
Change only: {authorized scientific, annotation, routing or rendering changes}.
Preserve: {correct objects, relations, directions, labels, semantic codes, layout regions and typography}.
Current problem -> required correction: {observable error, exact desired result}.
Scientific invariants: {sources, destinations, ordered edges, conditions and meaningful geometry}.
Affected text, verbatim: {only labels that change}.
Routing or layout permission: {affected line/region; where labels or objects may move; accurate anchors and available whitespace}.
Rendering: {confirmed style and relevant adaptation; on an authorized style change use the newly selected style}.
Exclusions: {selected style exclusions and user requirements}.
Keep all unaffected regions and the three distinct mark roles—driver fill, process outline and pathway arrow—unchanged.
```

Do not change unrelated regions during a local edit. For substantial layout changes, identify what may move rather than freezing everything. Do not call generation merely to record feedback or maintain this skill.

## Correct one relationship or arrow

```text
Correct only the specified connection in the supplied figure.
Current error: {wrong source/target/direction, false junction, or route crossing exact words}.
Correct relation: {actual source} -> {actual target}, meaning {physical transfer or causal effect}.
Remove: {the entire incorrect segment and its orphan arrowhead; identify by location and nearby labels}.
Draw: {one replacement route, source tail and target arrowhead; describe visible source/target geometry and a free corridor}.
Keep independent neighboring branches separate. Preserve {specific correct paths and labels}.
Use {the existing pathway class and its exact mark}; keep the corresponding legend sample consistent.
Do not add a duplicate connection, change the scientific relation, remove the dynamic process or replace it with a static symbol. Keep all unaffected content and the confirmed style.
```

Use coordinates as supplementary anchors only after inspecting the actual image and dimensions. Identify scientific anchors by objects, boundaries, or nodes. After correction, trace the whole source-to-target route, not just the new arrowhead.

## Switch style or correct style drift

```text
Use case: style-transfer.
Scientific content to preserve: {objects, layers, main chain, feedback edges, label wording, pathway endpoints and semantic codes}.
Requested style: {confirmed style ID/name, recorded for production and not printed}.
Apply: {selected rendering paragraph and scene-specific adaptation}.
Main visible cue: {color planes / continuous shading / fine structural lines / supported relief / selective material texture}.
Reduce the competing cue: {the rendering feature causing the current style drift}.
Keep informative geometry and mechanisms. Change visual treatment rather than reducing information. Text, legend marks and directional overlays remain flat, crisp and legible.
Preserve {viewpoint/layout if required for comparison}; allow {only justified local moves for readability}.
Do not add a title or explanatory paragraphs.
```

Do not prescribe a fixed generation count. Edit specific failures and recheck without repeatedly redrawing approved content. Correct wrong legends/relationships before evaluating rendering.

## Apply across subjects

- **Surface/subsurface processes:** derive entities and interfaces from evidence; use cuts for pathways/contact. Draw physical channels separately from explanatory arrows. Styles alter surfaces, not destinations.
- **State/intervention comparisons:** keep comparable objects, viewpoints, and codes; identify changed locations and conditions rather than relying on global brightness differences.
- **Industrial macro transport:** retain equipment and conduit volume; use independent flat paths for material direction. Branches, returns, and handoffs follow the actual process without internal electronic mechanisms.

These are organizational methods, not facts to add automatically. Do not depict objects, relationships, or stages unsupported by the current material.
