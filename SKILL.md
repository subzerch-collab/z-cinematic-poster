---
name: z-cinematic-poster
description: Turn a supplied portrait into a refined black-gold cinematic 3:4 poster or 1:1 avatar while preserving the same person's facial identity. Use for beauty, fashion, luxury, profile-image, or atmospheric editorial campaigns.
metadata:
  short-description: 将人物图做成高级感黑金海报或头像
---

# Cinematic Black-Gold Poster

Author: zero

Create a text-free, person-led black-gold cinematic editorial image from the user's portrait. Default to a vertical 3:4 poster; switch to a square 1:1 avatar when the user says avatar, profile image, headshot, 头像, or 1:1. The user normally needs only to upload a portrait and name a scene, mood, campaign theme, or output mode. Treat all rules below as defaults; do not make the user repeat them.

## Defaults

- Treat identity as the only non-negotiable invariant from the source portrait. Preserve the same person's facial structure and recognition cues: face shape and proportions, eye shape and spacing, brows, nose, lips, jawline, skin tone, apparent age, hairline, and distinguishing features. Do not preserve the original pose, crop, gaze, head tilt, expression, clothing, or accessories merely because they appear in the reference.
- Treat poor source lighting as damage to correct, not a look to preserve. If the portrait is underexposed, backlit, unevenly lit, color-cast, noisy, or covered by a large facial shadow, reconstruct clean facial illumination: a soft flattering key plus gentle fill, readable detail in both eyes and both sides of the face, natural luminous skin tone, controlled highlights, and enough soft shadow to retain three-dimensional form. Do not copy crushed shadows or brighten the face into a flat, pale, plastic mask.
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

## Output modes

- **Poster — default:** vertical 3:4, natural bust or half-body, with enough surrounding design to read as a finished campaign poster.
- **Avatar — on request:** square 1:1, close portrait or head-and-shoulders composition. Keep the full hair silhouette, chin, neck, and enough shoulders visible for believable anatomy. Center the face inside a circular-crop-safe area, keep eyes near the upper-middle rather than the top edge, and let the head and shoulders dominate the frame. Use layered black-gold material, halo, mist, light, and particles close behind and around the person instead of distant scenery or empty margins. Keep optical effects away from the eyes, nose, and mouth so identity stays immediately readable.

## Workflow

Inspect the supplied image as an identity reference, not as a pose, crop, exposure, or color-grade template. First assess whether facial information is obscured by darkness, hard shadow, glare, noise, or color cast; separate stable recognition cues from these photographic defects. Use any supplied poster only as a style reference. Choose and reconstruct the front, three-quarter, or side-facing pose that best serves the scene while preserving the same person.

For the visual treatment and scene-specific compositions, read [references/black-gold-campaign.md](references/black-gold-campaign.md). Build a concise generation prompt from the user's scene plus the defaults above. Before returning, compare the generated face with the reference and check: unmistakably the same person; the requested 3:4 or 1:1 aspect ratio; full uncropped head; natural anatomy; evenly readable facial illumination without crushed shadows; unified subject/background lighting; a visible soft double-exposure effect; and crisp high-detail foreground and mid-ground materials. For an avatar, also preview the composition as a circular crop and confirm the face, hair, chin, and key gold details remain intact. If identity has drifted or the corrected face is still dark, do not accept the image: regenerate with a softer brighter key, stronger fill, simpler facial effects, stronger identity language, and the face occupying more of the frame. A single side-view or severely obscured face may require inference for unseen features; keep the closest reliable scene-compatible angle or ask for an additional view instead of claiming an uncertain match.

## User-facing invocation

The user can simply upload a portrait and write one short line, for example:

> Use $z-cinematic-poster to turn this portrait into a premium black-gold poster.

Chinese is equally supported:

> 用 $z-cinematic-poster，把这张人物图做成高级感黑金海报。

They may optionally add a location, outfit, or emotion. Everything else is handled by default.

For a square avatar:

> Use $z-cinematic-poster to turn this portrait into a premium 1:1 black-gold avatar.

Chinese:

> 用 $z-cinematic-poster，把这张人物图做成 1:1 高级感黑金头像。
