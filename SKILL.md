---
name: z-cinematic-poster
description: Turn a supplied portrait into a refined black-gold cinematic image in a confirmed standard or custom aspect ratio while preserving the same person's facial identity. Use for beauty, fashion, luxury, profile-image, or atmospheric editorial campaigns.
metadata:
  short-description: 将人物图做成高级感黑金海报或头像
---

# z-cinematic-poster

Author: zero

Create a text-free, person-led black-gold cinematic editorial image from the user's portrait. Treat all visual rules below as defaults; do not make the user repeat them. Do not choose the canvas ratio on the user's behalf.

## Defaults

- Treat identity as the only non-negotiable invariant from the source portrait. Preserve the same person's structural recognition cues: face shape and proportions, eye shape and spacing, brows, nose, lips, jawline, apparent age, hairline, ethnicity, and base skin tone. Acne, acne marks, red dots, brown spots, freckles, pigmentation, dark patches, surface scars, and other skin-surface marks are not identity anchors and must be removed by default unless the user explicitly asks to keep one. Beauty-grade brightening and rosy color correction are allowed, but must not turn the person into someone else. Do not preserve the original pose, crop, gaze, head tilt, expression, clothing, or accessories merely because they appear in the reference.
- Treat expression as editable facial-muscle state, not identity. Unless the user requests another mood, replace a tired, blank, sad, tense, or listless expression with a natural happy, lively, approachable expression: relaxed brows, alert engaged eyes with clean catchlights, a subtle cheek lift, and gently raised mouth corners. Prefer an elegant closed-mouth or softly parted smile over a broad grin when the source does not reliably show the teeth. Preserve the person's exact eye shape, brow shape, nose, lip volume and contours, philtrum, jaw, face proportions, and other recognition cues; never enlarge the eyes, redraw the mouth, invent prominent teeth, or create a generic smiling face.
- Treat poor source lighting as damage to correct, not a look to preserve. If the portrait is underexposed, backlit, unevenly lit, color-cast, noisy, or covered by a large facial shadow, reconstruct clean facial illumination: a soft flattering key plus gentle fill, readable detail in both eyes and both sides of the face, natural luminous skin tone, controlled highlights, and enough soft shadow to retain three-dimensional form. Do not copy crushed shadows or brighten the face into a flat, pale, plastic mask.
- Apply a clearly visible high-end beauty-campaign finish by default, not a barely perceptible cleanup. Make the face bright, milky-translucent, silky-smooth, hydrated, spotless, and softly rosy, with continuous tonal gradients and controlled dewy highlights on the forehead, upper cheeks, nose, cupid's bow, and lips. Fully remove every visible tear track, dark fine line, under-eye crease, isolated red or brown dot, uneven pigmentation, spot, freckle, acne mark, blemish mark, surface scar, patch of redness, rough area, dry texture, mottled shadow, enlarged pore, orange-peel texture, camera grain, and sharpening grit; do not leave faint residual marks. At normal viewing size and in a close face crop, forehead, temples, both cheeks, under-eyes, nose, the area around the mouth, and chin must read as polished, even-toned skin with no individually recognizable mark, pore, or granular texture. Retain realism through facial form, subsurface color variation, and controlled light rather than visible pore or blemish detail. Add makeup that is immediately visible at first glance: refined full-coverage base, shaped brows, clean eyeliner or eye definition, separated lashes, healthy blush, subtle contour and highlight, softly colored glossy lips, polished hair, and overall grooming. Preserve facial geometry, eye/nose/lip shape, apparent age, ethnicity, hairline, and the person's overall identity. Beauty must come from skin finish, makeup, grooming, expression, and light—not from changing who the person is.
- Keep the primary facial landmarks optically sharp at the highest supported native resolution. The irises, catchlights, eyelashes, brows, nostril edges, lip line, and hair strands must have clean focus and precise edges, while facial skin stays smooth, continuous, and free of visible pore or grain detail. Apply detail selectively to landmarks only—never global sharpening, clarity, film grain, skin microcontrast, or high-frequency texture across the face. Never apply soft focus, motion blur, diffusion, bloom, haze, double exposure, denoise smearing, or glow across the central face; restrict those effects to the background, hair perimeter, outer silhouette, and secondary afterimage.
- Freely reconstruct a scene-appropriate front, three-quarter, or profile view. A side-facing or lowered head may become front-facing, raised, turned, or differently posed. Re-render the head, neck, shoulders, and body as one coherent photographed pose; never stretch, rotate, paste, or warp the original face.
- Adapt the wardrobe by default: replace ordinary, mismatched, or distracting clothing with a scene-appropriate black or black-gold editorial look using believable fabric and tailoring. Preserve the original outfit only when the user asks. Do not alter identity or anatomy while changing clothes.
- Default to a natural bust or half-body. Never invent a full body from a head-only reference. Keep the whole head in frame with breathing room, and render believable adult proportions.
- Build one coherent photographed or designed space: matching perspective, light direction, color grade, restrained haze, reflections, and depth-aware overlap. The subject must never look pasted onto the background.
- Use rich smoky bronze, amber, and sunset-gold midtones with black only as contrast. Do not leave broad empty black areas or make the whole frame muddy/dark.
- Make the image feel premium and atmospheric: a visible but soft partial double exposure or horizontal face/hair drag, golden rim/bloom, localized mist, fine gold dust, and a few irregular fading gold traces. Keep the primary face crisp and recognizable; never create a second readable face, wireframe, rigid ring, glitter overlay, or global blur.
- Respect a named location and time. Do not substitute a generic interior when the user asks for an exterior.
- If no location is requested, default to a designed black-gold poster environment rather than a literal lake or room: layered flowing gold ribbons, satin or liquid-metal curves, luminous arcs, fine particles, polished reflections, and matte/gloss contrast arranged around and behind the person.
- Render at the highest native resolution and quality the image tool supports. Keep the background materially legible: foreground and mid-ground forms must show clean microtexture, clean contours, controlled highlights, and layered depth; soften only the far distance and optical-effect edges. Never turn most of the backdrop into low-detail fog, smeared bokeh, compression artifacts, or low-resolution mush.
- Keep the scene detailed but subordinate to the person. No text, logo, watermark, border, or UI unless requested.

## Aspect-ratio gate

Establish the output ratio before generating anything. If the user has not already stated a ratio or exact dimensions, stop and ask this one concise question in the user's language, then wait for the answer:

> 请选择输出比例：1:1 头像、3:4 竖版海报、9:16 全屏竖版、16:9 横版海报、4:3 横版海报，或自定义比例/尺寸。

English:

> Choose an output ratio: 1:1 avatar, 3:4 vertical poster, 9:16 full-screen vertical, 16:9 landscape poster, 4:3 landscape poster, or a custom ratio/size.

Do not call the image-generation tool before the user selects. If the user already supplied one of these ratios or custom dimensions, do not ask again. Deliver exactly one final image per invocation. In Codex and any environment that automatically surfaces image-tool results, make exactly one image-generation or image-edit call for the entire invocation. Do not create a visible first draft, retry, repair pass, variation, batch, or second candidate. If the user requests several ratios, ask which single ratio to make first.

After selection, use the matching composition:

- **1:1 avatar:** close portrait or head-and-shoulders composition. Keep the full hair silhouette, chin, neck, and enough shoulders visible for believable anatomy. Center the face inside a circular-crop-safe area and keep optical effects away from the eyes, nose, and mouth.
- **3:4 vertical poster:** person-led bust or half-body editorial composition with enough surrounding design to read as a finished campaign poster.
- **9:16 full-screen vertical:** mobile-first portrait composition with the subject dominant and key face, hair, and gold accents away from extreme top and bottom interface-safe edges. Do not stretch a 3:4 layout or fill the extra height with empty black space.
- **16:9 landscape poster:** use a bust, half-body, or source-supported wider pose. Balance the opposite side with layered material, light, reflection, haze, or restrained afterimage rather than a blank scenic field.
- **4:3 landscape poster:** use a tighter editorial landscape composition than 16:9, keeping the person and black-gold design in close visual dialogue without oversized empty margins.
- **Custom:** honor the exact requested ratio. If the user gives pixel dimensions, preserve their ratio and request the closest or highest supported native resolution; never claim exact pixel dimensions when the image tool cannot provide them.

## Single-call refined-final protocol

Image-tool calls are user-visible in Codex even when the accompanying text calls them drafts. Therefore, complete the refinement plan before generation and treat the sole image call as the refined-final render.

- Before calling the image tool, inspect the source and build one complete final brief covering identity, expression, anatomy, ratio, crop, clothing, facial relighting, skin cleanup, under-eye repair, visible makeup, face sharpness, subject/background integration, black-gold materials, and exclusions.
- Request one output only. Do not use batch, variation, comparison, or multi-output mode. Make exactly one image-generation or edit call, even if the first result could be improved.
- Never describe an image-tool result as private or intermediate when the tool or client can surface it. Non-image reasoning, source inspection, and prompt preparation may remain internal; an actual image call may not.
- Do not make a second image call to retouch the first result in the same invocation. A requested revision is a new user-directed invocation and may create one replacement image only.
- If a tool unexpectedly returns a collection, select a single asset before any manual attachment when the interface permits; never attach the collection again. Do not trigger another generation attempt.
- The final response must contain one image card and one image asset. Do not also show the source, a before/after pair, alternatives, contact sheets, or duplicate links unless the user explicitly asks for comparison in a separate request. Provide only one final download link if a link is needed.

## Workflow

Inspect the supplied image as an identity reference, not as a pose, crop, exposure, or color-grade template. First assess whether facial information is obscured by darkness, hard shadow, glare, noise, or color cast; separate stable recognition cues from these photographic defects. Use any supplied poster only as a style reference. Choose and reconstruct the front, three-quarter, or side-facing pose that best serves the scene while preserving the same person.

For the visual treatment and ratio-specific composition, read [references/black-gold-campaign.md](references/black-gold-campaign.md). Before generation, convert the user's scene, confirmed ratio, and defaults above into one comprehensive refined-final prompt. Use the checklist as preflight instructions inside that prompt: unmistakably the same person; requested or naturally happy expression; exact aspect ratio; full uncropped head; natural anatomy; crisp eyes and facial landmarks without sharpened skin texture; evenly readable facial illumination; bright milky-translucent skin with a soft rosy undertone, smooth hydration, and continuous poreless-looking gradients; no isolated red, brown, or gray blemish dot, acne residue, dark spot, freckle, pigmentation patch, visible grain, enlarged pore, orange-peel texture, tear trough, eye bag, orange-brown under-eye rim, dark crease, tear track, or surface scar; makeup obvious at first glance; unified subject/background lighting; and optical effects outside the central face. Then make one image call only and return that result once. Do not call the image tool again for inspection-driven repair in the same invocation. A single side-view or severely obscured face may require inference for unseen features; choose the closest reliable scene-compatible angle or ask for an additional view before generation instead of claiming an uncertain match.

## User-facing invocation

The user can simply upload a portrait and invoke the skill. If they omit the ratio, ask the aspect-ratio question above before generating. For example:

> Use $z-cinematic-poster to turn this portrait into a premium black-gold poster.

Chinese is equally supported:

> 用 $z-cinematic-poster，把这张人物图做成高级感黑金海报。

They may optionally add a ratio, location, outfit, or emotion. Everything else is handled by default.

For a square avatar:

> Use $z-cinematic-poster to turn this portrait into a premium 1:1 black-gold avatar.

Chinese:

> 用 $z-cinematic-poster，把这张人物图做成 1:1 高级感黑金头像。
