# Design guide

Design quality comes from decisions that fit the product, not from a recognizable set of effects. Help the user understand, act, and feel the intended experience. Give the interface a coherent identity without making familiar tasks harder.

This is the authoritative source of general design principles for this guide. Explicit requirements and the product's established design system take precedence over generic preferences. Accessibility, truthful content, and correct behavior are constraints, not optional finishing touches.

## Start with the outcome

Identify or infer the user, primary task, first focal point, next action, and constraints that materially affect the change. Use actual content and realistic data; a layout that works only with short sample labels is unfinished.

Choose composition and density for the current surface:

- **Persuade:** make the proposition credible and the decision clear.
- **Operate:** bring the task, relevant data, and frequent actions within reach.
- **Read:** support comprehension, scanning, and navigation.
- **Experience:** let the work, media, or artifact carry the attention.

These are lenses, not templates. A product can use several. A utility may work best with its input and result visible immediately; a marketing page may need a demonstration and evidence before its call to action. Neither automatically needs a dashboard shell or a hero followed by three feature cards.

Match effort to scope. Fix a local spacing or contrast problem directly. For a new product or structural redesign, clarify the main journey and content relationships before detailed styling. Ask only when an unresolved decision materially changes the result; otherwise use the available evidence and proceed.

## Establish what can change

| Task | Starting point | Design freedom |
| --- | --- | --- |
| New interface | Product purpose, audience, platform, content, and any brand commitments | Choose a suitable visual direction and a compact system. |
| Improve existing UI | Shipped behavior, components, tokens, assets, and product design documentation | Improve the requested surface while preserving identity, navigation, content model, and behavior outside scope. |
| Explicit redesign | Product truth, required functionality, accessibility, and confirmed brand commitments | Reconsider composition and visual language coherently; change flows only within the requested scope. |

A missing design document does not make an established product a blank canvas. Reuse its components and semantic tokens; preserve deliberate differences between surfaces. Record durable decisions in the product's existing design documentation when useful, without creating a new documentation system for a small fix.

## Give the design an intention

When a new direction is needed, connect its desired feeling to concrete choices. For example: “Help readers compare complex material calmly: readable text columns, clear section headings, a quiet palette, and strong comparison alignment.” This is more actionable than “make it modern and premium.”

Draw identity from the subject, audience, content, brand, and environment. An expressive exhibit and a clinical scheduling tool need different emphasis. Novelty is optional; specificity and coherence matter. Keep standard controls recognizable and put expression where it improves recognition, understanding, trust, emotion, or the experience itself.

Use references to answer a design question. Real product flows are stronger evidence for task behavior than isolated concept shots; editorial and art-direction references can inform composition and mood. Extract why a choice works in its context rather than copying another product's shell. Research is optional when the existing evidence already supports the decision.

## Build hierarchy before decoration

Arrange content in the order users need it. Establish the main focal point and distinguish primary actions from alternatives. Use typography, proximity, alignment, proportion, spacing, and tonal contrast to make relationships visible before adding boxes and effects.

Use the **lowest sufficient visual containment**: try spacing and alignment first, then a tonal surface or divider, then a border or container when it clarifies a meaningful boundary. A card suits a distinct object or independently actionable group; it is not the default wrapper for every heading and paragraph. Elevation usually communicates floating or overlapping UI. A modal changes interaction and needs a task reason; it is not simply a stronger visual container.

For example, a settings page with six outlined cards may read more clearly as named sections with aligned labels and spacing. A selectable product collection may genuinely benefit from cards. Decide from the relationships and actions, not from a blanket rule against cards.

## Compose layout around real work

Use a shared alignment logic and a small spacing scale. Keep related items closer than unrelated sections. Size fields, reading columns, and work areas for their content rather than stretching every element to the available width.

Density follows the task: frequent professional work needs efficient scanning and reachable actions; reading needs comfortable measures; expressive surfaces may need generous space. Whitespace should establish grouping, rhythm, or emphasis. If a page feels empty, examine its proportions, shell, and hierarchy before adding content.

Keep navigation understandable and frequent actions discoverable. Reveal secondary complexity when it becomes relevant. Reserve space for persistent controls and ensure sticky headers, toolbars, and notices cannot cover content or focused inputs.

## Make typography do useful work

Choose fonts for legibility, language coverage, role, environment, loading cost, and intended character. System fonts and familiar neutral families can be excellent choices; display faces need a reason and readable supporting text. One family can carry a strong hierarchy. Add another only when the roles benefit.

Define a small set of distinct text roles with consistent sizes, weights, and line heights. Keep prose at a comfortable reading width; approximately 45–75 characters per line is a useful starting point, not a universal limit. Use aligned numeric presentation when users compare values. Check small labels, ambiguous glyphs, mixed scripts, and text enlargement.

Copy is part of the interface. Use the user's vocabulary, specific action labels, and consistent names across a flow. “Save changes” tells more than “Submit.” Keep labels visible when needed; remove repeated explanations before adding helper text. Do not invent metrics, testimonials, or capabilities to make a layout look complete.

## Use color, shape, and imagery with purpose

Reuse or define semantic roles for text, surfaces, boundaries, actions, focus, and status. Give colors stable meanings. In charts, combine color with labels, shapes, or patterns. Check contrast on the actual background, including image overlays, translucent surfaces, and every supported theme.

Shape and elevation should express a coherent material and interaction language. Use a small radius scale suited to the product and visually consistent nested corners. Choose emphasis deliberately: if everything is bright, oversized, rounded, or elevated, nothing has priority.

Imagery can explain the product, show evidence, or create an intended experience. Preserve meaningful proportions and reserve its layout space. A conspicuous logo or illustration often needs a quiet surround; repeated brand marks can compete with the content. Gradients, textures, shadows, and glow are legitimate when they contribute to the chosen visual language or communicate a state.

## Recognize generic AI aesthetics

The failure is an interchangeable design: the same blue-purple gradient, rounded card grid, oversized hero, glow, decorative badge, and generous empty bands applied to unrelated products. Replacing that kit with mandatory cream backgrounds, serif headings, sharp corners, or dark neon simply creates another default.

Ask of a prominent choice: **What does this help the user understand, do, feel, recognize, or trust here?** A reason can be functional, editorial, cultural, emotional, or expressive. It need not be purely utilitarian, but it should belong to this product.

If the interface feels generic, diagnose its content and composition first. Replace a generic feature grid with a meaningful comparison, expose a tool's real interaction, or let a gallery's work lead. Changing the accent color alone cannot fix an unsuitable structure. Preserve a deliberate gradient or familiar typeface when it serves the design.

After a coherent pass, remove UI whose removal does not harm comprehension, task success, accessibility, trust, or intended expression. Look for redundant labels, repeated status, nested containers, decorative icons, duplicate calls to action, and unsupported sections. The goal is useful visual economy, not compulsory minimalism.

## Design interaction and recovery

Make actions discoverable and communicate what happened. Include the states relevant to the feature: focus, pressed, selected, disabled, loading, empty, success, error, and recovery. Long operations need truthful progress or an honest waiting state; errors should identify the problem and offer a useful next action. Preserve entered data where possible.

Protect user context: focus, cursor, selection, scroll position, and familiar navigation should survive ordinary editing. Provide an understandable way back or an inverse for reversible actions; use confirmation or undo where the consequence warrants it.

Motion should explain change, maintain spatial continuity, provide feedback, or support intentional expression. Respect reduced motion, avoid false activity, and keep important content accessible without an animation completing. Favor stable layout and responsive controls over effects that add latency or distraction.

## Adapt to the viewport and input

Change structure when content stops fitting; do not merely shrink desktop UI. Decide what wraps, stacks, remains visible, or moves behind progressive disclosure. Preserve reading order and access to important tasks. Test long names, large values, missing data, localization, and enlarged text.

Support the platform's input and navigation conventions. Web UI needs keyboard access and visible focus; touch UI needs usable target sizes and alternatives to hover or precise dragging. On mobile, account for safe areas, the on-screen keyboard, back navigation, and reachable primary actions. Allow intentional scrolling for wide data or canvases without causing accidental page overflow.

## Treat accessibility as design quality

Use semantic structure, accessible names, persistent form labels, and a logical focus order. Keep focus visible and unobscured, and make interactions operable with keyboard and assistive technology where applicable. Explain validation near the affected field and announce significant state changes appropriately.

For web work, use WCAG 2.2 AA as a baseline: normally at least 4.5:1 contrast for text, 3:1 for qualifying large text, and 3:1 for meaningful control boundaries and visual indicators where required. Meet applicable target-size requirements and prefer comfortably sized touch areas. Follow native accessibility guidance on mobile. Do not sacrifice readability, zoom, contrast, or control access for visual restraint.

## Critique the rendered result

For a meaningful visual change, inspect the actual render or supplied visual evidence when available and authorized. Source review alone cannot establish composition quality. Compare before and after at the same viewport when refining existing UI; cover representative compact and wide layouts and the states affected by the change.

Use a short review:

- Is the intended task apparent, and is the next action easy to find?
- Does the hierarchy survive real content, smaller screens, and text enlargement?
- Are alignment, density, typography, color, shape, and component behavior coherent?
- Do interaction and recovery states work without clipping, occlusion, unexpected movement, or unreadable contrast?
- Does the expression belong to this product, and can unnecessary UI be removed?

Separate observable defects from taste preferences. Fix the few highest-impact findings together and confirm the fixes; continue only when a concrete issue remains. Use existing checks for objective failures, but do not mistake a passing build or automated audit for visual approval. If rendering or interaction verification is unavailable, state what remains unverified instead of claiming that the UI has been visually checked.
