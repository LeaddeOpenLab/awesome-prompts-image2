# Image 2.5 to Product Video: Asset Workflow

Use Image 2.5 to prepare consistent product keyframes before sending them into an image-to-video workflow.

**Pipeline:** approved product brief → master keyframe → scene variants → motion clip → verified narration and localization.

## Lock the brief

```text
Product:
Audience:
Single benefit:
Required product details:
Details that must not change:
Setting and camera framing:
Aspect ratio:
Final call to action:
```

## Master keyframe prompt

```text
Create a production-ready first frame for a [DURATION]-second product video.

Product: [PRODUCT]
Composition: [SHOT SIZE, ANGLE, SUBJECT POSITION]
Environment: [SETTING]
Lighting: [DIRECTION AND QUALITY]
Brand constraints: [COLORS, MATERIALS, LOGO RULES]
Motion space: leave clear space toward [DIRECTION] for [ACTION].

Preserve the exact product shape, controls, proportions, label placement,
materials, and color. Do not add text, accessories, duplicate products,
hands, reflections, or packaging unless specified.
```

Approve product fidelity before generating scene variants. Do not use a motion prompt to repair the wrong product geometry.

## Variant rules

- Reuse the approved master as a reference.
- Change one variable at a time: angle, environment, or action.
- Preserve product proportions, materials, controls, and brand colors.
- Keep important text outside generated pixels.
- Leave clean composition space for captions or presenter overlays.

## Handoff to video

Use the approved frame with a motion-focused prompt from the [Seedance library](https://github.com/LeaddeOpenLab/awesome-prompts-seedance). After the visual result is approved, add sourced narration and multilingual delivery with a document-first workflow such as [Leadde.ai](https://leadde.ai/?utm_source=github&utm_medium=guide&utm_campaign=image-product-assets).

Record the exact model/version, input image, prompt, date, aspect ratio, output, and correction prompt.

