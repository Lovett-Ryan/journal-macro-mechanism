---
name: journal-macro-mechanism
description: "Create, redraw, or edit 2.5D macro-scene mechanism figures for scientific journals. Review a text-and-layout skeleton before generating the full figure; optionally add approved local detail views and deliver raster scenes with editable Visio annotations. For environmental, urban, engineering, and industrial scenes; excludes microscopic biochemical mechanisms and internal electronic-device operation."
---

# Journal Macro Mechanism

Explain research through recognizable scenes, credible spatial relationships, complete mechanisms, and clear legends. All styles share the scientific content and information structure; the confirmed style controls form, surface detail, materials, and lighting.

Start with the [style catalog](references/style-catalog.md). Use [composition, annotations, and legends](references/style-guide.md) for shared rules, [content extraction and mechanism design](references/mechanism-design.md) for paper redraws or complex mechanisms, [prompt templates](references/prompt-templates.md) for generation and editing, and [review, annotation removal, and Visio assembly](references/review-and-visio.md) for skeleton review and editable delivery.

Read the [local detail view module](references/local-detail-views.md) only after the annotated main figure has passed user review and local views have been enabled. Do not load that module, its prompts, or layout examples during initial main-figure generation.

## Scope

- Depict object placement, interactions, material or energy transfer, spatial processes, stages, and interventions in macro scenes, including natural environments, cities, agriculture, ecology, industry, and transport.
- Exclude molecules, cells, proteins, biochemical reactions, circuits, chips, PCBs, and the internal structure or operation of electronic devices.
- Judge scope by the subject and explanatory scale. The external form, deployment, and system connections of macroscopic equipment are allowed. Naming a substance or flux beside a macro process does not constitute a microscopic reaction diagram.
- A user's request for a "micro view" within this skill means a local enlargement of a macro object's structure, interface, or physical process. Increase supported physical detail without expanding into the excluded subjects.
- For excluded subjects, explain the boundary and use an approach appropriate to the user's task; do not silently change the research topic.

## Confirm the style before drawing

1. Read the current [style catalog](references/style-catalog.md) at the start of each drawing task and check for an existing choice covering the figure, batch, or project.
2. If the user names a style, ID, sufficiently specific custom treatment, or an applicable prior choice, briefly acknowledge it and proceed. Record custom overrides. Content corrections to the same figure retain the confirmed style.
3. Otherwise, present every catalog style with a one-sentence distinction in the user's current language and ask for a choice. Wait for an actual response before writing the final generation prompt or calling the generator. A recommendation, preselection, or timeout is not confirmation.
4. Extract research content while waiting. Once confirmed, read the shared guide and selected style file. Load other styles only for an explicit comparison, switch, or mixture.
5. Record the scope of the choice. Confirm again for tasks outside that scope, without repeatedly asking during revisions of the same figure.

Content analysis, reverse analysis of images or prompts, and style-document maintenance do not require style selection.

## Default figure conventions

- Full workflow: text-and-layout skeleton → user review → complete annotated mechanism figure → user review → optional local-object selection → derive a clean main scene and selected local images → assemble native Visio annotations. Without local views, use the single-main-figure workflow. For raster-only requests, deliver the approved complete figure. Respect narrower requests for analysis, prompts, or documentation.
- The skeleton is a reviewable content and layout design, not a separate branch for generating a text-free reference scene. Generate the complete figure from the same scientific specification, object hierarchy, text, and relationships. Do not generate an empty scene and then try to supply its mechanism by pasting on a skeleton.
- Editable delivery retains the textured scene as a raster and rebuilds text, boxes, leaders, mechanism arrows, and legends as native Visio objects. Do not use Illustrator tracing, whole-scene SVG reconstruction, or object-by-object scene vectorization as intermediate steps.
- Finish the Visio stage when all requested content has been inserted and the native file saved. Subsequent formatting belongs to the user. Do not default to iterative checks or adjustments of font sizes, wrapping, box dimensions, opacity, spacing, or alignment, or require preview export. Refine these only on an additional user request.
- No overall title inside the artwork. Keep paper titles, figure titles, and sources in captions or production records. Necessary panel letters, region names, and legend headers are allowed. Honor an explicit request for an in-figure title.
- Give key objects and processes short nearby labels. The legend explains the actual semantic encoding. Object names, process labels, and legends have distinct roles and cannot replace each other.
- Preserve the full supported mechanism while reducing decoration and repeated text. Do not place abstract paragraphs, background statistics, or projection discussions in the figure. Use short, highly transparent white-backed notes only where they add necessary explanation.
- These conventions apply to every style. No topic's objects, palette, legend categories, layout, or particular figure becomes a universal template.

## Isolate inputs by stage

Build a separate, complete prompt and image-input list for the initial annotated main figure. Include only its scientific content, objects, labels, legend, style, and confirmed corrections. Do not submit the full conversation, future-stage plans, or a historical edit chain as generation input.

- Before main-figure approval, do not load the local-view module or put future detail subjects, locator circles, correspondence dashes, reserved panels, or assembly requirements in the initial prompt. Do not introduce them even through negative instructions. Record a known future request only as a production to-do.
- Exclude examples, layout images, and assets supplied for later local views from the initial call. Specify necessary current-stage images by explicit paths instead of automatically including unrelated recent images.
- Keep genuine cutaways and layers required by the main scene; these are not independent detail views. Do not reserve space or reduce main-figure content for future functionality.
- Give every later generation call its own prompt and input list, containing only what that asset needs. Save the actual submitted versions. This isolates tool prompts and supplied assets; it does not erase the conversation context.

## Workflow

### 1. Extract the scientific scope

Create a concise drawing specification: core question, scene boundary, required objects and hierarchy, directed relationships, exact labels, evidence and conditions, output language and format, and confirmed style and its scope.

For paper redraws, figure reconstruction, and multi-process reviews, read [mechanism design](references/mechanism-design.md). Inspect the relevant original figure, caption, and mechanism-related text; determine which figure and processes are being redrawn. With only an abstract, stay within its evidence. Use the supplied material fully to understand the study, then turn relevant claims into visible objects and paths rather than printing all the source text.

Check coverage as "central claim → object/process → label/legend." Maintain an object-label inventory, directed-relation table, and semantic-code table as the common source for the skeleton and generation prompt. Do not invent unknown relationships, values, or directions. Ask only about gaps affecting correctness or key composition, while progressing on settled content.

### 2. Organize the scene and submit the skeleton

Derive layout and semantic colors from the current research. The scene carries objects and spatial relationships; flat graphics carry transfer, causality, regulation, and feedback. Follow the [shared guide](references/style-guide.md).

- Establish subject positions, depth, necessary side faces, cutaways, and material interfaces, with space for labels and paths. Use cutaways and panels for explanatory need, without a fixed block base or panel count. Select optional local views after main-figure approval.
- Name individually recognizable objects relevant to the mechanism. Keep neighboring objects and media distinguishable.
- Preserve physical channels, pipes, and structures as entities. Keep abstract pathways flat, distinguishing physical transfer from causal feedback rather than rendering both as pipes.
- Specify each path's source, target, meaning, direction, and conditions. Do not connect parallel sources as a false conversion chain. Check each feedback edge; for actual circulation also check viewpoint and rotation.
- Where these roles exist, prefer pale solid driver marks, thin outlined process marks, and colored pathway arrows. Derive categories from the subject and cross-check legend samples against the scene. Object labels alone do not constitute a legend.
- Place labels directly beside their objects. Use highly transparent white-backed secondary notes without leaders. Add a short leader only when nearby placement remains ambiguous.
- Separate states or regions that produce opposite effects. Define signs, ±, and dashed codes with evidence and a legend; symbols must not conceal unknown causality.
- Beautification and style changes preserve scientific structure, coverage, and established encoding. Schematic scale, shading, and arrow thickness must not imply unsupported quantities.

Use the [review requirements](references/review-and-visio.md) to present spatial layout, object hierarchy, exact labels and nearby positions, path endpoints, and legend styles. A complex figure may have a simple wireframe preview, but not another generated text-free scene. Hierarchy supports scientific organization and annotation association; it does not require minimum-unit vector decomposition.

Show the skeleton and request review of content, hierarchy, label positions, and relationships. Unless the user explicitly changes this review requirement, wait for approval of that version before generating the complete figure. Revise the skeleton when requested. Write the final tool prompt after approval; a confirmed style is not skeleton approval.

### 3. Generate the complete figure from the approved skeleton

Use the [prompt templates](references/prompt-templates.md). Specify scientific content, directed relationships, composition, selected rendering, exact text, and legend encoding separately. Apply the selected style's complex-figure guidance and exclusions to the actual objects; a style or journal name alone is insufficient. Do not load competing styles' restrictions.

- Put the reviewed skeleton and original scientific specification into one full prompt. Generate a complete figure containing scene, material treatment, short labels, boxes, essential leaders, mechanism arrows, and legend together. Do not paste the skeleton onto a reference image or require literal tracing of a skeleton preview.
- Respect the reviewed regions and object-label associations, while allowing small whitespace adjustments for aesthetics and readability. Approximate coordinates are not pixel constraints. Return to skeleton review if the main layout, scientific connections, or key information must change.
- Inspect every input image and state whether it supplies science, appearance, or the edit target. Existing figures may be task-specific inputs without becoming permanent dependencies.
- Prefer built-in `image_gen` for raster generation and editing, following the available `imagegen` skill and its saving conventions. No separate API key is needed. If unavailable, explain the limitation; use a CLI/API route only when explicitly chosen by the user.
- For edits, specify the observed problem, exact change, and preserved content. When allowing major movement, do not simultaneously freeze every position. Separate style and scientific corrections where useful; do not prescribe a fixed number of generation rounds.
- Default to a white or very pale background. Follow requested language, typeface, transparency, framing, and format; otherwise use a clear conventional sans-serif font.
- Do not introduce OCR services or token configuration. A request for a fully vector scene exceeds this hybrid raster-scene/editable-annotation workflow; determine an appropriate approach for that request rather than describing the hybrid as fully vector.

### 4. Check, correct, and submit the complete figure

A successful tool response is not proof of correctness. Check science and paths first, then encoding, layout, and style.

| Check | Acceptance criteria |
| --- | --- |
| Scientific coverage | Required objects, stages, main chain, feedbacks, and branches are present; no invented conclusions or mixed conditions/time scales |
| Objects and labels | Objects are visible and recognizable; nearby names match; terminology, symbols, and spelling are correct |
| Causality and endpoints | Paths start and finish at the right anchors; parallel outputs stay parallel; static icons do not replace circulation or feedback |
| Legend correspondence | Fill, outline, arrows, and symbols match actual uses; all codes are explained and all legend entries used |
| Readability | Paths avoid words; no orphan heads, false junctions, or leader tangles; no tiny text or paragraph panels used to force a fit |
| Space and states | Interfaces, cutaways, and occlusion are credible; opposing effects have distinguishable states or conditions |
| Style | The selected style's visible cues are present; texture, lighting, and detail do not obstruct the explanation |
| Restraint | No default overall title or unnecessary abstract/statistical/discussion boxes; required labels and legend remain complete |
| Intended size | Objects, text, and arrows remain legible at the intended size; no important content is clipped |

Write corrections as "current error → correct source/target or depiction → available route → preserved content." Fix misleading meaning before crowding or rendering. For persistent path errors, move labels, reroute, or use a scientifically useful local view. Do not delete key processes or arrows, or replace a dynamic mechanism with a letter or static icon, merely to avoid generation difficulty. Record unresolved issues honestly.

Show the checked complete figure. Unless the user explicitly changes the review requirement, begin annotation removal and Visio assembly only after approval of that version. Internal checks, tool success, or silence are not approval. Raster-only requests finish here. Reuse an already approved figure without repeating its skeleton or review.

At this review stage, offer local views when they would explain otherwise unclear structures or processes. Do not generate them early. If already requested, record opt-in without asking again. Load the local module only after main approval and opt-in; confirm objects and explanatory focus before generating that branch's assets.

### 5. Derive clean scenes and assemble Visio

For editable delivery, read [review and Visio assembly](references/review-and-visio.md).

- If local views are enabled, generate the clean main scene and selected annotation-free local images as independent assets using the delayed module. Extend the canvas outside the main figure and add native locators and a few no-arrow dashed correspondence lines. Decide this layout now, without redrawing the initial main figure to reserve space.
- Supply the approved full figure as the actual input for targeted annotation removal. Remove every word, box, leader, mechanism arrow, standalone explanatory symbol, and the entire legend; restore covered scenery. Preserve viewpoint, frame, objects, interfaces, materials, and style. A newly imagined text-only background is insufficient.
- Check for residual text, frames, arrows, and duplicate legend marks; compare object positions and materials. Preserve real rivers, smoke, layers, and natural process forms. Rebuild only explanatory overlays as editable objects.
- Calibrate anchors against the actual clean image. Embed and lock it at the bottom of Visio; recreate all text, boxes, leaders, mechanism arrows, and legend natively. Group by object or process while preserving individual editability within groups.
- After insertion and saving, perform one overall confirmation: scenes and annotations are displayed, required content is present, explanatory objects are native/editable, and the file is usable. Reuse a current application view or user confirmation. Do not repeatedly reopen, try-edit text, drag arrows, or test legend items. Finish and leave format refinement to the user. Corrupt files, missing scenes, or absent required content still need repair.

### 6. Save, deliver, and incorporate feedback

- Follow existing project paths and names; otherwise use `Figure/macro-mechanism/`. Version revised figures unless overwrite was requested.
- Save the skeleton, approved complete figure, clean main image, selected local images, and native Visio file according to scope. Record versions, actual formats, and dimensions. Retain the approved original and each image separately.
- Save actual full prompts and edit chains, style ID/custom overrides, and each input image's role and path. For complex figures, retain coverage, relation, and encoding checks as production records rather than artwork.
- Record the actual versions approved at both review stages and the final annotation inventory and image-coordinate mapping. For local views, record selected subjects and source anchors. Use truthful states: awaiting review, approved figure, awaiting local-object selection when applicable, generating assets, assembling Visio, and workflow complete. Later user formatting is not an unfinished task.
- Put attribution in captions or production records as appropriate. Verify specific submission requirements rather than claiming compliance with a journal.
- For documentation or feedback-only requests, record the feedback and update relevant files without automatically editing or regenerating images. Distinguish implemented rules from unchanged earlier artwork.
- Deliver file links and a concise account of changes and meaningful checks. State clearly that scenes remain rasters and text, frames, leaders, arrows, and legends are editable native objects.
