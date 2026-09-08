# z-cinematic-poster

Turn a portrait into a polished black-gold cinematic poster while keeping the person recognizable and naturally integrated into the design.

**Author:** zero

## What it does

- Preserves facial identity while allowing a scene-appropriate expression and pose.
- Defaults to a vertical 3:4 bust or half-body composition with natural anatomy.
- Replaces ordinary clothing with refined black or black-gold editorial wardrobe unless preservation is requested.
- Builds high-detail abstract or environmental backgrounds with amber-gold light, metallic texture, haze, fine particles, and soft partial double exposure.
- Keeps the subject and background in one coherent light, perspective, color grade, and depth system.
- Generates without text, logos, or watermarks by default.

## Examples

The people shown below are fictional and were generated specifically for this repository.

| Source portrait | Abstract black-gold poster |
| --- | --- |
| ![Fictional source portrait 1](examples/example-01-source.png) | ![Abstract black-gold result](examples/example-01-poster.png) |

| Source portrait | Environmental black-gold poster |
| --- | --- |
| ![Fictional source portrait 2](examples/example-02-source.png) | ![Environmental black-gold result](examples/example-02-poster.png) |

## Requirements

- Codex with Skills support.
- An available image-generation tool that supports image references or identity-preserving edits.
- A clear portrait works best. Only use images you have permission to process.

Image fidelity, pixel dimensions, and exact likeness depend on the available image model and the quality of the source portrait. The skill requests the highest native quality supported but cannot create detail absent from a very small or heavily compressed source.

## Install

Copy or clone this repository into your Codex skills directory:

```text
~/.codex/skills/z-cinematic-poster/
```

The installed directory must contain `SKILL.md`, `agents/`, and `references/` at its top level. Restart or refresh Codex if the skill does not appear immediately.

## Use

Upload a portrait, then invoke the skill with one sentence:

```text
Use $z-cinematic-poster to turn this portrait into a premium black-gold poster.
```

中文：

```text
用 $z-cinematic-poster，把这张人物图做成高级感黑金海报。
```

Optional details can be added naturally:

```text
Use $z-cinematic-poster with a rain-wet city at blue hour and a tailored formal outfit.
```

You do not need to repeat the identity, anatomy, lighting, double-exposure, resolution, or integration rules; they are built into the skill.

## Repository structure

```text
z-cinematic-poster/
├── SKILL.md
├── agents/openai.yaml
├── references/black-gold-campaign.md
├── examples/
└── LICENSE
```

## Safety and rights

Do not publish portraits without the subject's permission. Do not redistribute watermarked reference images, brand assets, or copyrighted photographs you do not control. Style references guide visual language only; the skill explicitly excludes copied logos, text, and watermarks from outputs.

## License

Released under the MIT License. See [LICENSE](LICENSE).

---

## 中文简介

`z-cinematic-poster` 可将人物参考图转化为 3:4 高级黑金电影海报。默认保持人物五官与整体相貌，自动调整合适的半身比例、姿态、服装、光影、柔和双曝和背景质感。用户通常只需上传人物图并输入一句调用语。
