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

## Facial relighting and source repair

The portrait supplies identity, not exposure. When the source is dim, backlit, uneven, strongly color-cast, noisy, or partly hidden by hard shadow:

- Reconstruct the face under clean studio-quality light rather than reproducing the source defect.
- Use a soft frontal or three-quarter amber key with a broad neutral-warm fill. Both eyes, cheeks, the nose, lips, and jaw should remain readable.
- Keep gentle modeled shadow under the cheekbones, nose, and jaw so the face stays dimensional; avoid flat front-flash lighting.
- Recover a natural skin tone and restrained catchlights without whitening the person, changing complexion, over-smoothing pores, or inventing new facial structure.
- Keep atmospheric darkness, double exposure, haze, and gold effects around the hair and outer silhouette. Do not let them darken or obscure the central face.
- If the reference contains too little reliable facial information, prefer the closest supported angle or request another portrait rather than hallucinating identity.

## Identity, anatomy, and wardrobe

- Preserve the same person's distinctive face shape and proportions, eye shape and spacing, brows, nose, lips, jaw, skin tone, age presentation, hairline, and identifying features.
- Do not inherit the source angle by default. A side-facing or lowered head may become front-facing, raised, three-quarter, profile, or differently posed when the composition benefits.
- Re-render the head, neck, shoulders, and body as one coherent photographed pose. Never stretch, rotate, paste, or warp the original face.
- Do not beautify the person into a different face. Avoid changing eye size, nose structure, lip shape, jaw shape, apparent age, ethnicity, or other recognition cues.
- Keep the whole head and hair silhouette in frame with breathing room.
- Default to a believable bust or half-body. Do not infer a full body from a head-only reference. Keep adult head, neck, shoulders, torso, arms, and hands proportionate.
- Unless the user asks to preserve the original outfit, replace ordinary or scene-mismatched clothing with a coherent editorial wardrobe. Prefer tailored black formalwear, sculptural black silk, satin, velvet, or restrained black-gold couture. Keep fabric construction realistic, tasteful, and subordinate to the face.
- Removable accessories may be removed unless requested. Never remove permanent distinguishing features.

## Beauty, skin, and makeup

Use a polished editorial finish by default without asking the user for another setting. If they name a makeup style or intensity, follow it.

- Refine temporary blemishes, patchy redness, excess shine, under-eye fatigue, dry lips, and stray facial hairs while retaining pores, fine skin texture, natural tonal variation, and age-appropriate detail.
- Preserve complexion and stable identifying features such as moles, freckles, scars, eyelid structure, smile lines, and hairline unless the user explicitly requests removal.
- Use a natural-to-polished makeup presence appropriate to the person's styling and campaign mood: clean base, groomed brows, defined eyes and lashes, subtle contour and highlight, healthy cheek tone, and finished lips. Makeup should be visible enough to feel intentional but not costume-like unless requested.
- For a sharper or more handsome treatment, favor clean matte-to-satin skin, controlled brow and eye definition, understated lips, tidy facial hair when present, sculpting through light, and precise hair grooming.
- For a softer or more glamorous treatment, favor luminous satin skin, refined eye and lash definition, restrained contour, blush and highlight, harmonized lip color, and polished hair.
- Do not assume or change gender presentation. Choose the finish from the source styling and requested mood, and allow the user to override it.
- Never enlarge eyes, shrink the nose, narrow the jaw, inflate lips, erase all pores, whiten skin, de-age aggressively, or reshape the face to create attractiveness.

## Background modes

### Abstract poster — default

Use two or three material families: flowing metallic-gold ribbons, black satin dunes, liquid-metal folds, luminous arcs or light curtains, polished reflections, and sparse star-like particles. Combine large elegant curves with fine surface detail. Avoid stock gradients, hard frames, symmetrical wire graphics, and excessive glitter.

### Named environment

When the user names a location or time, make it unmistakable through its materials, horizon, weather, practical light, and reflections. Apply the black-gold visual system without replacing the requested place with a generic room. Keep scenery close and subordinate to the portrait rather than turning the result into a travel photograph.

## Ratio-specific composition

- **1:1:** use a close portrait or head-and-shoulders crop with the full hair silhouette, chin, neck, and enough shoulders visible. Keep the face in the circular safe area. Place detailed black-gold materials and atmosphere close to the silhouette; keep effects outside the eyes-nose-mouth zone.
- **3:4:** use a bust or half-body vertical editorial layout. Surround the person with layered design without reducing them to a small figure.
- **9:16:** use a mobile-first vertical layout. Keep important facial and decorative details away from extreme top and bottom edges, distribute authored material through the extra height, and avoid empty black extension.
- **16:9:** use the horizontal direction to create visual dialogue between the person and designed light/material layers. If the person is offset, give the opposite side meaningful gold structure, reflections, atmosphere, or afterimage rather than generic scenery or vacancy.
- **4:3:** use a compact horizontal bust or half-body layout with denser interaction between subject and design than 16:9.
- **Custom:** design directly for the requested proportions instead of stretching or cropping a standard composition. When pixel dimensions are provided, preserve the ratio and use the highest supported native output size.

## Compact prompt assembly

Build a concise prompt containing only:

1. the supplied image's role as the identity reference, with identity locked but original pose, gaze, head angle, crop, expression, clothing, and accessories unlocked;
2. the confirmed output ratio—1:1, 3:4, 9:16, 16:9, 4:3, or custom—plus its ratio-specific framing, supported body scope, and a newly reconstructed scene-appropriate front, three-quarter, or profile pose;
3. requested scene or the abstract poster default;
4. scene-appropriate wardrobe replacement unless preservation is requested;
5. shared amber-gold lighting and depth-aware integration, with corrected soft key-and-fill facial illumination when the source is dark or uneven;
6. polished editorial skin, grooming, and scene-appropriate makeup that improve attractiveness without changing facial geometry or identifying features;
7. one soft partial double exposure plus restrained gold accents;
8. crisp face and high-detail foreground/mid-ground; and
9. exclusions: no text, logo, watermark, identity drift, duplicate face, pasted cutout, anatomy distortion, plastic skin, face reshaping, rigid frame, global blur, or low-resolution background.

Do not expose this expanded brief unless the user asks for the prompt. The user-facing invocation should remain one sentence.

## Final check

Confirm that the result uses the user's confirmed ratio, is unmistakably the same person after any angle or pose change, has an evenly exposed and naturally dimensional face, shows refined real-looking skin and intentional makeup or grooming, is naturally proportioned, appropriately dressed, integrated into one coherent black-gold space, visibly but softly double-exposed, detailed rather than muddy, and free of text or watermarks. For a 1:1 avatar, also confirm it survives a circular crop without losing the face, hair, chin, or defining gold details. If the face has drifted, remains crushed by shadow, looks over-retouched, or uses the wrong ratio, reject and regenerate rather than presenting it as successful.
