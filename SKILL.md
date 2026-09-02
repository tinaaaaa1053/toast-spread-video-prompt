---
name: toast-spread-video-prompt
description: Generate copy-ready English prompts for Google Flow or similar text-to-video models in which any specified object is placed on toast, completely transformed into a spreadable material, and spread in one continuous ASMR macro shot. Use for 任意物体涂抹面包、吐司解压视频、ASMR crushing-and-spreading prompts, prompt variants, or repairs to clips with jump cuts, leftover chunks, uneven coatings, or inconsistent materials.
---

# Toast Spread Video Prompt

Turn the user's object into a visually coherent toast-spreading sequence. Preserve the object's recognizable identity in its initial shape, transformation behavior, colors, final spread, and sounds; do not merely substitute its name into a fixed template.

## Build the material plan

Infer reasonable defaults when the user supplies only an object name. Ask a question only when the object itself is ambiguous or the user requires an exact count, palette, duration, or direction that cannot be inferred.

Before drafting, decide internally:

- object count and scale: one large object or roughly three to five smaller objects that fit fully on the toast;
- signature geometry and surface cues that make the object immediately recognizable;
- two to four restrained colors, highlights, translucency, iridescence, or glow;
- a staged deformation from intact object to spreadable medium;
- the resulting medium, such as cream, paste, gel, jelly, glaze, or thin film;
- three synchronized sound layers: object breakdown, material release, and knife-on-toast friction.

Read [references/material-logic.md](references/material-logic.md) when choosing transformation, texture, color, or sound behavior for a new object category, or when repairing a failed prompt.

The six user-authored source prompts are preserved verbatim in [references/original-prompts.md](references/original-prompts.md). Read them only when the user asks for the originals, wants a style comparison, or requests a revision anchored to a specific source example; the material logic in this file remains authoritative for new prompts.

## Write one continuous visual sequence

Produce one polished, copy-ready English prompt unless the user requests another language, multiple variants, or commentary. Use natural cinematic prose rather than exposed placeholders.

Keep this chronology:

1. Establish a hyper-realistic macro ASMR shot, fixed camera, fully visible thick-cut golden toast, soft lighting, and one uninterrupted take.
2. Show one hand gently placing the intact object or objects on the toast, then withdrawing. Describe the object's distinctive form and material under the light.
3. Introduce the butter knife and use short, readable presses from one side to transform the objects completely. Describe two or three observable stages rather than jumping directly from solid to cream.
4. State that all original rigid structure is gone before spreading begins, with no chunks, shards, shells, rings, fragments, or unbroken pieces remaining. Override this only if the user explicitly wants retained texture.
5. Make the knife perform exactly one smooth spreading pass from one edge of the toast to the opposite edge. Keep the knife at a low angle with steady pressure and show the entire path on camera.
6. Describe the final coating's thickness, coverage, color behavior, sheen, and contrast with the toast.
7. End with object-specific ASMR sounds and concise continuity constraints.

The crushing may require several short presses; “one single continuous motion” applies specifically to the final spreading pass. Do not describe the whole clip as one knife motion if that would contradict the crushing stage.

## Preserve identity through transformation

Carry the object's signature features into the spread instead of inventing unrelated effects:

- geometry becomes cracks, ribbons, cellular ripples, layered streaks, or banding;
- surface character becomes matte, glossy, metallic, crystalline, pearlescent, translucent, or airy texture;
- the original palette becomes a controlled gradient, not a muddy rainbow;
- distinctive internal features become inclusions or light patterns only when they fully dissolve into the medium.

For a hard or inedible object, frame liquefaction as a surreal visual transformation. Keep hands safe and the result fantastical; do not imply that the real object is edible or can physically melt under a table knife.

## Enforce continuity

State observable constraints positively and concretely. Include the applicable items in the prompt:

- fully fixed camera, stable framing, constant lighting and toast position;
- one continuous take with no cuts, jump cuts, time skips, speed ramps, or hidden transitions;
- exactly one toast, one knife, and only the necessary hands;
- no duplicated, respawned, floating, or prematurely disappearing objects;
- no warped fingers, morphing knife, changing toast shape, text, captions, logos, or music;
- crushing visibly finishes before spreading begins;
- the spreading pass stays in contact with the toast, moves in one direction, reaches the opposite edge, and does not reverse or restart;
- no residual solids or thick piles when a smooth coating is requested.

Avoid bloating the ending with every possible defect. Select the constraints most likely to fail for the chosen object while always retaining fixed camera, no cuts, complete transformation, and one uninterrupted spreading pass.

## Match coating style to the material

Choose one clear final target:

- thin film: low knife angle, delicate translucent or metallic sheen, no raised buildup;
- smooth layer: even opaque or semi-transparent coating with gentle streaks;
- fluffy layer: soft, airy ridges without intact crumbs or shells;
- jelly layer: glossy ripples and translucent color bands without solid inclusions;
- molten layer: dense flowing patterns and luminous gradients, contained entirely on the toast.

Do not demand both an extremely thin film and a thick, fluffy or heavily rippled finish.

## Final check

Before returning the prompt, verify that:

- the intact object, breakdown, released medium, final coating, and sounds all describe the same material concept;
- count, colors, direction, thickness, and lighting do not change mid-prompt;
- the entire action can fit in one visible composition;
- the prompt distinguishes crushing presses from the single spreading stroke;
- the final text contains no bracketed variables or unexplained alternatives.

Return the finished prompt directly. If the user asked for help choosing settings or reports a failed generation, add only a brief note after the prompt explaining the relevant adjustment.
