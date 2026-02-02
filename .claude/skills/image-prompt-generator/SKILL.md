---
name: image-prompt-generator
description: |
  Generate professional AI image prompts for YouTube thumbnails and visuals.
  This skill should be used when users say "create thumbnail", "image prompt",
  "thumbnail prompt", "generate image", or "make thumbnail".
---

# Image Prompt Generator

Create professional AI image prompts with photography expertise built-in.

## What This Skill Does

- Guides non-experts through professional image concepts
- Suggests best options with simple explanations
- Generates copy-paste ready prompts for Midjourney/DALL-E/Ideogram
- Optimizes for YouTube thumbnail CTR

## What This Skill Does NOT Do

- Generate actual images (outputs prompts only)
- Edit existing images
- Create video content (use `video-prompt-generator` skill)

---

## Workflow

### Step 1: Ask MCQ Questions (One at a Time)

**IMPORTANT:** Ask one question → Give suggestion based on their context → Wait for answer

---

**Q1: Image Purpose**
```
🎨 What's this image for?

A) YouTube Thumbnail (16:9 ratio) — Most common, optimized for clicks
B) YouTube Banner (2560x1440) — Channel branding
C) Video Background/B-roll — Scene imagery
D) Social Media Post (1:1 square) — Instagram, Facebook
E) Custom (describe your need)
```

---

**Q2: Video Topic**
```
📝 What's your video topic/script about?

[User types topic OR references previous script-writer output]
```

---

**Q3: Image Mood**
```
🎭 What MOOD should the image create?

💡 For [their topic], I recommend [X] because [reason]

A) 😲 Shocking/Surprising — Grabs attention, great for facts/reveals
B) 🤔 Curious/Intriguing — Makes viewers want to know more
C) 😊 Happy/Positive — Builds trust, good for tutorials
D) 😨 Fear/Urgency — Drives clicks, good for warnings/mistakes
E) 🔥 Exciting/Energetic — High energy, good for tech/gaming
F) 😌 Calm/Professional — Builds authority, good for education
G) Let me choose the best mood for your topic
```

---

**Q4: Color Scheme**
```
🎨 Color scheme preference?

💡 High contrast colors get 30% more clicks on YouTube

A) 🔴🟡 Red + Yellow — Maximum attention, urgency (Top CTR)
B) 🔵⚪ Blue + White — Trust, professional, tech
C) 🟢⚫ Green + Black — Money, growth, success
D) 🟣🟡 Purple + Gold — Luxury, premium, unique
E) 🟠⚫ Orange + Dark — Energy, excitement, gaming
F) 🌈 Vibrant Multi-color — Fun, entertainment
G) Let me choose best colors for your niche
```

---

**Q5: Camera Angle**
```
📷 Camera angle/perspective?

💡 This affects how viewers FEEL about the subject

A) 👁️ Eye Level — Relatable, friendly, equal (Most common)
B) ⬆️ Low Angle (looking up) — Powerful, dominant, impressive
C) ⬇️ High Angle (looking down) — Overview, vulnerable, small
D) 🔍 Close-up/Macro — Detail focus, intensity, emotion
E) 🌅 Wide/Panoramic — Context, scale, environment
F) 🎯 Dutch Angle (tilted) — Dynamic, tension, action
G) Let me choose the best angle
```

---

**Q6: Lighting Style**
```
💡 Lighting style?

💡 Lighting creates 60% of the image mood

A) ☀️ Bright & Natural — Clean, trustworthy, friendly (Most versatile)
B) 🌅 Golden Hour — Warm, cinematic, inspiring
C) 🎭 Dramatic Side Light — Bold, professional, serious
D) 💜 Neon/RGB Glow — Tech, gaming, futuristic
E) 🌙 Dark & Moody — Mystery, thriller, intense
F) 📸 Studio Soft Light — Product shots, professional, clean
G) Let me choose best lighting
```

---

**Q7: Background Style**
```
🖼️ Background style?

💡 Background should support, not distract from main subject

A) 🔵 Solid Color Gradient — Clean, text-friendly (Best for thumbnails)
B) 🌆 Realistic Environment — Context, story, relatable
C) ✨ Abstract/Particles — Modern, tech, dynamic
D) 🌫️ Blurred/Bokeh — Focus on subject, professional
E) 🎮 Themed Scene — Gaming room, office, studio
F) ⬛ Pure Black/Dark — Dramatic, focus, premium
G) Let me choose best background
```

---

**Q8: Main Subject**
```
👤 What should be the MAIN subject/focus?

A) 👤 Person/Face — Expressing emotion (best for personal brands)
B) 🖥️ Product/Object — Device, tool, item being discussed
C) 📊 Text/Typography — Bold text as main element
D) 🎨 Conceptual/Symbol — Abstract representation of topic
E) 🔀 Split/Comparison — Two elements side by side
F) Describe your specific subject
```

---

**Q9: AI Tool Target**
```
🤖 Which AI tool will you use?

A) Midjourney — Best quality, artistic (Recommended)
B) DALL-E 3 — Good for text, realistic
C) Ideogram — Best for text in images
D) Stable Diffusion — Free, customizable
E) Leonardo AI — Good balance
F) Generate prompts for all tools
```

---

### Step 2: Generate Prompts

After collecting answers, generate prompts using this structure:

---

## Prompt Structure Formula

```
[Subject] + [Action/Pose] + [Environment/Background] + [Lighting] + [Color Scheme] + [Mood/Atmosphere] + [Camera Angle] + [Style Keywords] + [Technical Parameters]
```

---

## Output Template

```markdown
## 🎨 AI Image Prompts

**Topic:** [Topic]
**Purpose:** [Thumbnail/Banner/etc.]
**Mood:** [Selected mood]

---

### 🏆 MAIN PROMPT (Recommended)

**For Midjourney:**
```
[Complete optimized prompt]
--ar 16:9 --v 6 --s 250
```

**For DALL-E 3:**
```
[DALL-E optimized prompt]
```

**For Ideogram:**
```
[Ideogram optimized prompt with text instructions]
```

---

### 🔄 VARIATION PROMPTS

**Variation 1 - More Dramatic:**
```
[Alternative prompt]
```

**Variation 2 - More Minimal:**
```
[Alternative prompt]
```

**Variation 3 - Different Angle:**
```
[Alternative prompt]
```

---

### 📝 TEXT OVERLAY SUGGESTIONS

If adding text to thumbnail:
- **Main Text:** "[Suggested headline]"
- **Font Style:** [Bold sans-serif/etc.]
- **Placement:** [Top/Bottom/Side]
- **Color:** [Contrasting color]

---

### ⚙️ Technical Settings

| Setting | Value |
|---------|-------|
| Aspect Ratio | [16:9 / 1:1 / etc.] |
| Resolution | [1920x1080 / etc.] |
| Style | [Photorealistic / Illustrated / etc.] |

---

### 💡 Pro Tips

1. [Tip specific to their use case]
2. [Tip for better results]
3. [Common mistake to avoid]
```

---

## Niche-Specific Recommendations

### Tech & AI
- **Colors:** Blue + White, Neon accents
- **Lighting:** Dramatic side light or RGB glow
- **Background:** Abstract particles, dark gradient
- **Subject:** Product close-up or conceptual tech imagery

### Finance & Money
- **Colors:** Green + Gold, or Red + Black
- **Lighting:** Studio soft light
- **Background:** Solid gradient or luxury setting
- **Subject:** Money imagery, growth charts, success symbols

### Gaming
- **Colors:** Orange + Dark, Neon multi-color
- **Lighting:** RGB/Neon glow
- **Background:** Gaming setup, action scene
- **Subject:** Game characters, intense expressions

### Education
- **Colors:** Blue + White, calm palette
- **Lighting:** Bright natural or soft studio
- **Background:** Clean gradient, classroom subtle
- **Subject:** Person explaining, visual diagrams

### Entertainment/Facts
- **Colors:** Vibrant, high contrast
- **Lighting:** Dramatic for mystery, bright for fun
- **Background:** Themed to topic
- **Subject:** Shocking imagery, expressive faces

---

## Style Keywords Reference

### Photorealistic
`photorealistic, hyperrealistic, 8k, detailed, sharp focus, professional photography`

### Cinematic
`cinematic lighting, film grain, movie poster style, dramatic, epic`

### Modern/Clean
`minimalist, clean design, modern, sleek, professional`

### Artistic
`digital art, illustration, concept art, stylized`

### 3D Render
`3D render, octane render, unreal engine, CGI, smooth`

---

## Output Checklist

Before delivering:
- [ ] Prompt matches selected mood and colors
- [ ] Aspect ratio correct for purpose
- [ ] Multiple variations provided
- [ ] Tool-specific formatting applied
- [ ] Text overlay suggestions if thumbnail
- [ ] Pro tips relevant to their niche

---

## Reference Files

| File | When to Read |
|------|--------------|
| `references/prompt-formulas.md` | Detailed prompt structures by tool |
| `references/niche-styles.md` | Style guides by content niche |
