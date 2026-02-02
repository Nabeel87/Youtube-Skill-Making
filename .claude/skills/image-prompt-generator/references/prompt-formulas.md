# Prompt Formulas by AI Tool

Optimized prompt structures for each major AI image generator.

---

## Midjourney Prompts

### Basic Structure
```
[Subject], [Description], [Environment], [Lighting], [Style], [Mood] --ar [ratio] --v 6 --s [stylize]
```

### Parameters
| Parameter | Values | Purpose |
|-----------|--------|---------|
| `--ar` | 16:9, 1:1, 9:16 | Aspect ratio |
| `--v` | 5, 5.2, 6 | Version (6 is latest) |
| `--s` | 0-1000 | Stylize (higher = more artistic) |
| `--q` | 0.5, 1, 2 | Quality |
| `--c` | 0-100 | Chaos (variation) |
| `--no` | [element] | Exclude element |

### Thumbnail Formula
```
[Emotion expression] [person/subject], [action], [bold colors] background,
[lighting type], YouTube thumbnail style, high contrast, vibrant,
eye-catching, professional photography --ar 16:9 --v 6 --s 250
```

### Example Prompts

**Tech Review Thumbnail:**
```
young man with shocked surprised expression looking at glowing smartphone,
dramatic blue and orange lighting, dark gradient background with tech particles,
cinematic, YouTube thumbnail style, high contrast, 8k --ar 16:9 --v 6 --s 200
```

**Money/Finance Thumbnail:**
```
confident businessman holding stack of cash money, green and gold color scheme,
luxury dark background with subtle glow, dramatic studio lighting,
success wealth concept, YouTube thumbnail --ar 16:9 --v 6 --s 250
```

**Motivation Thumbnail:**
```
determined person silhouette against sunrise, orange and purple gradient sky,
inspirational epic atmosphere, cinematic lighting, motivational concept,
dramatic wide shot --ar 16:9 --v 6 --s 300
```

---

## DALL-E 3 Prompts

### Basic Structure
```
A [style] [image type] of [subject] [doing action] in [setting],
[lighting description], [color palette], [mood/atmosphere].
```

### Best Practices
- More natural language works better
- Be specific about text if including any
- Describe style explicitly (photorealistic, illustration, etc.)
- Include mood and atmosphere descriptions

### Example Prompts

**Tech Thumbnail:**
```
A photorealistic YouTube thumbnail showing a person with an amazed expression
looking at a glowing AI interface on their laptop screen. Dramatic blue and
cyan lighting from the screen illuminates their face. Dark background with
subtle tech particles. High contrast, vibrant colors, professional quality.
```

**Tutorial Thumbnail:**
```
A clean, professional YouTube thumbnail with a friendly person pointing at
a floating checklist graphic. Bright, well-lit studio environment.
Blue and white color scheme. Modern, trustworthy aesthetic.
Sharp focus, high quality photography style.
```

---

## Ideogram Prompts

### Best For
- Text-heavy thumbnails
- Logos and typography
- Text that needs to be readable

### Structure
```
[Image description], with text "[YOUR TEXT]" in [font style] [color] letters,
[placement], [background], [style]
```

### Example Prompts

**Thumbnail with Text:**
```
YouTube thumbnail, shocked person reacting, with bold text "YOU WON'T BELIEVE THIS"
in large white letters with red outline, centered, dark dramatic background
with light rays, high contrast, vibrant
```

**List Video Thumbnail:**
```
Clean YouTube thumbnail with large "TOP 10" text in bold red 3D letters,
golden glow effect, dark blue gradient background, professional design,
eye-catching typography
```

---

## Stable Diffusion Prompts

### Structure
```
[Subject], [Details], [Environment], [Lighting], [Style keywords], [Quality tags]

Negative prompt: [Things to avoid]
```

### Quality Tags
```
masterpiece, best quality, high resolution, 8k, detailed, sharp focus,
professional photography
```

### Negative Prompt Template
```
blurry, low quality, distorted, deformed, ugly, bad anatomy,
watermark, text, logo, oversaturated
```

### Example

**Prompt:**
```
professional YouTube thumbnail, person with excited expression,
holding glowing device, dramatic orange and blue lighting,
dark background with particles, cinematic, high contrast,
masterpiece, best quality, 8k, sharp focus
```

**Negative:**
```
blurry, low quality, distorted face, bad hands, watermark,
text, ugly, deformed
```

---

## Leonardo AI Prompts

### Structure
Similar to Midjourney but without parameters in prompt.

```
[Subject] [Action] [Environment] [Lighting] [Style] [Quality descriptors]
```

### Model Recommendations
| Use Case | Model |
|----------|-------|
| Photorealistic | Leonardo Diffusion XL |
| Artistic | DreamShaper |
| Characters | Absolute Reality |

### Example
```
Excited tech reviewer holding futuristic gadget, dramatic rim lighting,
dark studio background with blue accent lights, professional photography,
YouTube thumbnail style, high contrast, vibrant colors, 8k quality
```

---

## Universal Prompt Elements

### Emotion Keywords
| Emotion | Keywords |
|---------|----------|
| Shocked | surprised, amazed, jaw dropped, wide eyes, shocked expression |
| Happy | smiling, joyful, excited, cheerful, positive |
| Curious | intrigued, wondering, questioning look, raised eyebrow |
| Serious | focused, determined, confident, professional |
| Scared | worried, fearful, anxious, concerned |

### Lighting Keywords
| Type | Keywords |
|------|----------|
| Natural | natural lighting, daylight, sunlit, outdoor light |
| Studio | studio lighting, soft box, professional lighting |
| Dramatic | dramatic lighting, rim light, backlit, chiaroscuro |
| Neon | neon glow, RGB lighting, cyberpunk lights |
| Golden | golden hour, warm sunset, orange glow |

### Background Keywords
| Type | Keywords |
|------|----------|
| Gradient | smooth gradient, color gradient, fade background |
| Particles | floating particles, dust motes, sparkles, light rays |
| Bokeh | blurred background, bokeh lights, shallow depth |
| Dark | dark background, black void, shadows |
| Environment | office setting, studio, outdoor scene |

### Quality Boosters
```
8k, ultra detailed, high resolution, professional photography,
sharp focus, masterpiece, best quality, hyperrealistic
```

---

## Common Mistakes to Avoid

❌ **Too many subjects** - Keep focus on ONE main element
❌ **Conflicting styles** - Don't mix "cartoon" with "photorealistic"
❌ **Weak lighting description** - Always specify lighting type
❌ **No mood/atmosphere** - Add emotional context
❌ **Wrong aspect ratio** - Always match to platform (16:9 for YouTube)
❌ **Text in Midjourney** - Use Ideogram for text-heavy images
