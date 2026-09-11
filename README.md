# Krea 2 Angle Prompts

A set of angle prompts for Krea 2, written to keep a subject consistent across generations while changing the camera angle. Browse by angle, then copy any prompt directly into your workflow.

## What this is

Most prompt resources online are large, general-purpose lists where angle-specific prompts are scattered among hundreds of unrelated ones. This repository is focused entirely on camera angle: seventeen prompts covering vertical elevation and tilt (low angle, high angle, worm's-eye, bird's-eye, etc.) and horizontal orbit (front, three-quarter, profile, etc.).

## How it works

Each prompt describes camera position and framing in full sentences, not short tags. This matches how Krea 2's text encoder (Qwen3-VL) parses language, so descriptive sentences are interpreted more reliably than comma-separated keywords.

To use a prompt:

1. Pick an angle from the site or this repository.
2. Copy the prompt text.
3. Replace the subject description with your own, keeping the angle-specific wording intact.
4. Generate.

## Model compatibility

These prompts were written and tested against:

- Krea 2 Turbo (checkpoint)
- Qwen Image VAE
- Qwen3-VL text encoder

No LoRAs were used to produce the example images on the site.

They should also work reasonably well on other models that use natural-language text encoders (T5 or LLM-based), such as Qwen-Image, FLUX 1 and 2, Stable Diffusion 3 and 3.5, and DALL-E 3. They are less likely to work well on CLIP-only, tag-based models such as Pony Diffusion or classic SDXL/SD1.5 checkpoints, which expect short comma-separated tags rather than full sentences.

## Consistency notes

These prompts control camera angle. They do not guarantee identical output between runs. AI generation is not deterministic by default: the same prompt can still produce variation in pose or framing from one generation to the next. For closer consistency across a set, keep the subject description identical between prompts and consider using a fixed seed or a reference image.

## Contributing

Contributions of new angle prompts are welcome. To submit one:

1. Open a pull request or issue with the prompt text.
2. Include an example generated image if possible.
3. Follow the existing format (full-sentence description, no tags).

## License

The code in this repository has no license attached, meaning all rights are reserved by default. The prompt text and example content are licensed separately under CC BY-NC 4.0 (Attribution-NonCommercial). This allows reuse and remixing, provided credit is given and the material is not used commercially without permission. See `LICENSE.md` for details.
