---
name: z-cinematic-poster
description: Turn a supplied portrait into a refined 3:4 black-gold cinematic poster while preserving the person's likeness. Use for beauty, fashion, luxury, or atmospheric editorial campaigns.
metadata:
  short-description: 将人物图做成高级感黑金电影海报
---

# Cinematic Black-Gold Poster

Author: zero

Create a text-free, vertical 3:4, person-led black-gold cinematic editorial poster from the user's portrait. The user normally needs only to upload a portrait and name a scene, mood, or campaign theme. Treat all rules below as defaults; do not make the user repeat them.

## Defaults

- Preserve the person's recognizable facial identity. Expression, pose, face angle, clothing, and removable accessories may change to suit the scene, but do not turn them into a different person.
- Adapt the wardrobe by default: replace ordinary, mismatched, or distracting clothing with a scene-appropriate black or black-gold editorial look using believable fabric and tailoring. Preserve the original outfit only when the user asks. Do not alter identity or anatomy while changing clothes.
- Default to a natural bust or half-body. Never invent a full body from a head-only reference. Keep the whole head in frame with breathing room, and render believable adult proportions.
- Build one coherent photographed or designed space: matching perspective, light direction, color grade, restrained haze, reflections, and depth-aware overlap. The subject must never look pasted onto the background.
- Use rich smoky bronze, amber, and sunset-gold midtones with black only as contrast. Do not leave broad empty black areas or make the whole frame muddy/dark.
- Make the image feel premium and atmospheric: a visible but soft partial double exposure or horizontal face/hair drag, golden rim/bloom, localized mist, fine gold dust, and a few irregular fading gold traces. Keep the primary face crisp and recognizable; never create a second readable face, wireframe, rigid ring, glitter overlay, or global blur.
- Respect a named location and time. Do not substitute a generic interior when the user asks for an exterior.
- If no location is requested, default to a designed black-gold poster environment rather than a literal lake or room: layered flowing gold ribbons, satin or liquid-metal curves, luminous arcs, fine particles, polished reflections, and matte/gloss contrast arranged around and behind the person.
- Render at the highest native resolution and quality the image tool supports. Keep the background materially legible: foreground and mid-ground forms must show clean microtexture, clean contours, controlled highlights, and layered depth; soften only the far distance and optical-effect edges. Never turn most of the backdrop into low-detail fog, smeared bokeh, compression artifacts, or low-resolution mush.
- Keep the scene detailed but subordinate to the person. No text, logo, watermark, border, or UI unless requested.

## Workflow

Inspect the supplied image. Use it as the identity reference and use any supplied poster only as a style reference. Choose a front, three-quarter, or side-facing pose that fits the scene while preserving likeness.

For the visual treatment and scene-specific compositions, read [references/black-gold-campaign.md](references/black-gold-campaign.md). Build a concise generation prompt from the user's scene plus the defaults above. Before returning, check: vertical 3:4; full uncropped head; natural anatomy; unified subject/background lighting; a visible soft double-exposure effect; crisp high-detail foreground and mid-ground materials; and no identity drift.

## User-facing invocation

The user can simply upload a portrait and write one short line, for example:

> Use $z-cinematic-poster to turn this portrait into a premium black-gold poster.

Chinese is equally supported:

> 用 $z-cinematic-poster，把这张人物图做成高级感黑金海报。

They may optionally add a location, outfit, or emotion. Everything else is handled by default.
