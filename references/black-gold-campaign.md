# Black-gold cinematic campaign guide

Use this guide to turn the user's short request into a concrete image-generation brief. Treat identity as the only hard invariant from the source portrait. Preserve a scene, outfit, expression, or crop only when the user states it; otherwise rebuild them for the poster.

## Visual system

- **Palette:** smoky charcoal, dark bronze, amber, burnt orange, and sunset gold. Keep black as contrast rather than an empty dominant field.
- **Light:** use one motivated amber key and a gold rim. The same light must affect the face, hair, clothes, floor or surrounding materials.
- **Integration:** place visual elements behind the subject, grazing the silhouette, and sparingly across an outer hair, shoulder, or clothing edge. Match perspective, reflections, grain, shadow color, and atmospheric depth.
- **Optical hero:** use one visible but soft partial double exposure or horizontal afterimage around part of the hair, cheek edge, or shoulder. The primary face stays readable; never form a complete second face.
- **Supporting detail:** use one or two restrained effects such as an incomplete halo, broken gold filament, light streak, controlled bloom, localized mist, or fine illuminated particles. Let them fade asymmetrically.
- **Resolution:** keep the primary face, hair, fabric, foreground, and mid-ground sharp with clean microtexture. Soften only the far distance and optical transitions. Avoid low-detail fog, smeared bokeh, compression artifacts, or global blur.
- **Density:** build three depth planes and keep quiet areas authored with texture, reflections, light, or material detail. No large featureless black rectangle.

## Identity, anatomy, and wardrobe

- Preserve the same person's distinctive face shape and proportions, eye shape and spacing, brows, nose, lips, jaw, skin tone, age presentation, hairline, and identifying features.
- Do not inherit the source angle by default. A side-facing or lowered head may become front-facing, raised, three-quarter, profile, or differently posed when the composition benefits.
- Re-render the head, neck, shoulders, and body as one coherent photographed pose. Never stretch, rotate, paste, or warp the original face.
- Do not beautify the person into a different face. Avoid changing eye size, nose structure, lip shape, jaw shape, apparent age, ethnicity, or other recognition cues.
- Keep the whole head and hair silhouette in frame with breathing room.
- Default to a believable bust or half-body. Do not infer a full body from a head-only reference. Keep adult head, neck, shoulders, torso, arms, and hands proportionate.
- Unless the user asks to preserve the original outfit, replace ordinary or scene-mismatched clothing with a coherent editorial wardrobe. Prefer tailored black formalwear, sculptural black silk, satin, velvet, or restrained black-gold couture. Keep fabric construction realistic, tasteful, and subordinate to the face.
- Removable accessories may be removed unless requested. Never remove permanent distinguishing features.

## Background modes

### Abstract poster — default

Use two or three material families: flowing metallic-gold ribbons, black satin dunes, liquid-metal folds, luminous arcs or light curtains, polished reflections, and sparse star-like particles. Combine large elegant curves with fine surface detail. Avoid stock gradients, hard frames, symmetrical wire graphics, and excessive glitter.

### Named environment

When the user names a location or time, make it unmistakable through its materials, horizon, weather, practical light, and reflections. Apply the black-gold visual system without replacing the requested place with a generic room. Keep scenery close and subordinate to the portrait rather than turning the result into a travel photograph.

## Square avatar mode

Use this mode when the user asks for an avatar, profile image, headshot, 头像, or 1:1 output.

- Use a square 1:1 canvas with a close portrait or head-and-shoulders crop. Do not use a distant half-body composition.
- Keep the full hair silhouette, chin, neck, and enough shoulders visible to avoid a floating or oversized head.
- Keep the face centered within the inner circular safe area so the result still works when a platform crops the square into a circle.
- Put detailed black-gold materials and atmospheric effects close to the silhouette. Use an incomplete halo, soft gold rim, localized mist, fine particles, flowing metallic curves, or a restrained afterimage to balance the frame.
- Preserve crisp eyes and facial structure. Keep double exposure, light streaks, gold dust, and haze off the central eyes-nose-mouth recognition zone.
- Avoid text, distant landscape emphasis, large empty corners, hard rings, badge-like borders, and symmetrical decorative frames.

## Compact prompt assembly

Build a concise prompt containing only:

1. the supplied image's role as the identity reference, with identity locked but original pose, gaze, head angle, crop, expression, clothing, and accessories unlocked;
2. the requested output mode: vertical 3:4 poster, or square 1:1 circular-crop-safe avatar; include the supported body scope and a newly reconstructed scene-appropriate front, three-quarter, or profile pose;
3. requested scene or the abstract poster default;
4. scene-appropriate wardrobe replacement unless preservation is requested;
5. shared amber-gold lighting and depth-aware integration;
6. one soft partial double exposure plus restrained gold accents;
7. crisp face and high-detail foreground/mid-ground; and
8. exclusions: no text, logo, watermark, identity drift, duplicate face, pasted cutout, anatomy distortion, rigid frame, global blur, or low-resolution background.

Do not expose this expanded brief unless the user asks for the prompt. The user-facing invocation should remain one sentence.

## Final check

Confirm that the result uses the requested 3:4 or 1:1 ratio, is unmistakably the same person after any angle or pose change, naturally proportioned, appropriately dressed, integrated into one coherent black-gold space, visibly but softly double-exposed, detailed rather than muddy, and free of text or watermarks. For a 1:1 avatar, also confirm it survives a circular crop without losing the face, hair, chin, or defining gold details. If the face has drifted, reject and regenerate rather than presenting it as successful.
