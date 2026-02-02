---
name: voice-script-generator
description: |
  Convert YouTube scripts into TTS-optimized voiceover scripts for ElevenLabs, PlayHT, Murf, Edge TTS.
  This skill should be used when users say "create voice script", "voiceover for",
  "TTS script", "voice for script", "elevenlabs script", "optimize for speech", or "generate voiceover".
---

# Voice Script Generator

Create TTS-optimized voiceover scripts with audio production expertise built-in.

## What This Skill Does

- Acts as a professional voice director/audio producer
- Optimizes scripts for natural AI speech flow
- Adds pauses, emphasis markers, and pronunciation guides
- Generates copy-paste ready scripts for ElevenLabs, PlayHT, Murf, Edge TTS
- Explains audio terms in simple language

## What This Skill Does NOT Do

- Generate actual audio (outputs optimized text scripts)
- Clone voices or create voice profiles
- Write video scripts (use `script-writer` skill)
- Create video prompts (use `video-prompt-generator` skill)

---

## Workflow

### Step 1: Ask MCQ Questions (One at a Time)

**IMPORTANT:** Ask one question → Give suggestion based on their context → Wait for answer

---

**Q1: Voice Purpose**
```
🎙️ Kis cheez ke liye voice chahiye?

A) Full Video Voiceover — Complete script, start to end
B) Intro/Outro Only — Opening and closing narration
C) Specific Section — Paste or describe which part
D) Short Clips/Highlights — Key moments, sound bites
```

---

**Q2: Script Input**
```
📝 Apna script share karo:

💡 Options:
- Paste your full script below
- Reference previous script: "use my last script"
- Type topic for quick voiceover text

[User inputs their content]
```

---

**Q3: TTS Tool Selection**
```
🔊 Kaun sa TTS tool use karoge?

💡 Each tool has different capabilities - I'll optimize accordingly

A) ElevenLabs — Most natural, emotions, cloning capability ⭐ Best Quality
B) PlayHT — Great quality, 800+ voices, good emotions
C) Murf AI — Professional, business-focused, clean
D) Edge TTS — Free, Microsoft voices, decent quality
E) Google TTS — Free, basic but reliable, many languages
F) Coqui TTS — Free, open source, customizable
G) Multiple Tools — I'll compare results from different tools
H) Not Sure — Suggest best tool for my content type
```

---

**Q4: Voice Character**
```
🗣️ Voice character type?

💡 For [their content type], I recommend [X] because [reason]

A) 👨‍💼 Professional Male — Authority, business, finance, serious topics
B) 👩‍💼 Professional Female — Friendly authority, corporate, tutorials
C) 🧑 Young Male — Energetic, tech, gaming, casual, relatable
D) 👩 Young Female — Friendly, lifestyle, beauty, conversational
E) 🎙️ Deep Male — Documentary, dramatic narration, motivation
F) 👵 Mature/Warm — Trustworthy, educational, storytelling, comforting
G) 🤖 AI/Robotic — Tech content, futuristic, unique style
H) Let AI Suggest — Based on my content type
```

---

**Q5: Voice Emotion/Tone**
```
🎭 Voice emotion aur tone kaisa chahiye?

💡 This sets the overall feel of your voiceover

A) 😊 Friendly & Conversational — Natural, like talking to a friend
   Best for: Most YouTube content, tutorials, vlogs
B) 🎓 Professional & Authoritative — Confident, expert, business
   Best for: Finance, business, serious education
C) 🔥 Energetic & Excited — High energy, enthusiasm, hype
   Best for: Tech reveals, gaming, product launches
D) 😌 Calm & Soothing — Relaxed, peaceful, gentle
   Best for: Meditation, relaxation, ASMR, sleep content
E) 🎬 Dramatic & Cinematic — Intense, storytelling, powerful
   Best for: Documentaries, stories, movie-style narration
F) 💪 Motivational & Inspiring — Uplifting, encouraging, powerful
   Best for: Self-help, fitness, success content
G) 😄 Fun & Playful — Light, humorous, entertaining
   Best for: Entertainment, kids content, comedy
H) 🔀 Mixed — Different emotions for different sections
   Best for: Long-form content with varying moods
```

---

**Q6: Speaking Pace**
```
⚡ Speaking pace kitna chahiye?

💡 Average YouTube pace is 150-160 words/minute
   Pace affects how much viewers absorb

A) 🐢 Slow (120-130 wpm) — Clear, easy to follow, complex topics
   Best for: Tutorials, education, older audience, non-native speakers
B) 🚶 Medium (140-150 wpm) — Balanced, comfortable, natural ✅ Recommended
   Best for: Most content types, general audience
C) 🏃 Fast (160-170 wpm) — Energetic, keeps attention, younger audience
   Best for: Entertainment, tech, gaming, news
D) 🚀 Very Fast (180+ wpm) — High energy, excitement, intense
   Best for: Hype content, gaming highlights, excitement builds
E) 🔀 Variable — Slow for important parts, fast for energy sections
   Best for: Long-form content, storytelling, mixed pacing
```

---

**Q7: Accent Preference**
```
🌍 Accent preference?

💡 Accent affects audience connection and understanding

A) 🇺🇸 American English — Most global appeal, widely understood
B) 🇬🇧 British English — Sophisticated, professional, European appeal
C) 🇦🇺 Australian English — Friendly, casual, unique character
D) 🌐 Neutral/International — No strong accent, maximum clarity
E) 🇮🇳 Indian English — South Asian audience, regional connection
F) 🇨🇦 Canadian English — Friendly, neutral North American
G) Other — Specify your preference
```

---

**Q8: Pause Style**
```
⏸️ Pause style preference?

💡 Pauses help comprehension, add drama, and make speech natural
   Without pauses, AI voice sounds robotic and rushed

A) ⚡ Minimal Pauses — Fast-paced, energetic, no breaks
   Best for: Excitement, gaming, rapid content
B) 💬 Natural Pauses — Like normal conversation ✅ Recommended
   Best for: Most content, sounds human and natural
C) 🎭 Dramatic Pauses — Long pauses for emphasis and impact
   Best for: Motivation, storytelling, key reveals
D) 📚 Educational Pauses — Extra time to absorb information
   Best for: Tutorials, complex topics, learning content
E) 🤖 Let AI Optimize — Automatic pause placement
   Best for: Quick generation, trust the algorithm
```

---

**Q9: Special Requirements**
```
📊 Koi special requirements hain?

💡 These help me optimize the script correctly

A) 🔢 Numbers/Statistics Heavy — Need clear number pronunciation
   Example: "1,000,000" → "one million" or "ten lakh"
B) 🔬 Technical Terms — Need pronunciation guides for jargon
   Example: "API" → "A-P-I" or "nginx" → "engine-x"
C) 🌐 Multiple Languages — Non-English words in script
   Example: Hindi phrases, French names, etc.
D) ™️ Brand Names — Specific pronunciations needed
   Example: "Xiaomi" → "Shao-mee", "Huawei" → "Wah-way"
E) 🎭 Emotional Variations — Different tones in same script
   Example: Excited intro, calm explanation, urgent CTA
F) ✅ No Special Requirements — Standard script optimization
G) 📝 Multiple of Above — Specify which ones
```

---

### Step 2: Analyze & Optimize Script

After collecting answers, transform the script:

1. **Break into sections** - Hook, main content, CTA
2. **Add pause markers** - Based on preference (short/medium/long)
3. **Mark emphasis words** - Important terms, numbers, CTAs
4. **Add pronunciation guides** - Technical terms, names, foreign words
5. **Optimize sentence length** - Shorter = more natural speech
6. **Remove filler words** - Unless intentional for naturalness
7. **Add breathing points** - Natural places to pause

---

### Step 3: Generate Optimized Voice Script

Generate script using tool-specific formatting:

---

## Pause Marker System

| Marker | Duration | Usage |
|--------|----------|-------|
| `,` | 0.2-0.3s | Natural breath, clause break |
| `.` | 0.4-0.5s | Sentence end |
| `...` | 0.6-0.8s | Thoughtful pause, suspense |
| `[pause]` | 1.0s | Dramatic emphasis |
| `[long pause]` | 1.5-2.0s | Major section break |

---

## Emphasis System

| Marker | Effect | Example |
|--------|--------|---------|
| **CAPS** | Strong emphasis | "This is REALLY important" |
| `*word*` | Light emphasis | "This is *actually* useful" |
| `_word_` | Slower pronunciation | "That's _fascinating_" |

---

## Output Template

```markdown
## 🎙️ TTS-Optimized Voice Script

**Original Length:** [X] words
**Optimized Length:** [X] words
**Estimated Duration:** [X:XX] at [X] wpm
**Tool:** [Selected TTS tool]
**Voice Type:** [Selected voice]
**Emotion:** [Selected emotion]

---

### ⚙️ TTS SETTINGS

**For [Tool Name]:**
| Setting | Recommended Value |
|---------|-------------------|
| Voice | [Specific voice name] |
| Speed | [X.X] (based on pace preference) |
| Stability | [X.X] (for consistency) |
| Clarity | [X.X] (for articulation) |
| Style | [Emotion setting] |

---

### 🎬 SECTION 1: HOOK
**Duration:** ~[X] seconds
**Emotion:** [Emotion for this section]

```
[Optimized hook script with pause markers and emphasis]
```

**Voice Direction:** [How to deliver this section]

---

### 📖 SECTION 2: MAIN CONTENT
**Duration:** ~[X:XX]
**Emotion:** [Emotion for this section]

```
[Optimized main content with all markers]
```

**Voice Direction:** [Delivery notes]

---

### 🎯 SECTION 3: CTA (Call to Action)
**Duration:** ~[X] seconds
**Emotion:** [Emotion for this section]

```
[Optimized CTA with emphasis on action words]
```

**Voice Direction:** [How to deliver CTA]

---

### 📝 PRONUNCIATION GUIDE

| Word/Term | Pronunciation | Notes |
|-----------|---------------|-------|
| [Term 1] | [How to say it] | [Context] |
| [Term 2] | [How to say it] | [Context] |

---

### 🔢 NUMBERS GUIDE

| Original | Speak As | Why |
|----------|----------|-----|
| 1,000,000 | "one million" | Clearer for audience |
| 50% | "fifty percent" | Standard |
| $99 | "ninety-nine dollars" | Full pronunciation |

---

### 💡 PRO TIPS

1. **For [their tool]:** [Specific optimization tip]
2. **Pacing tip:** [How to handle speed variations]
3. **Common mistake:** [What to avoid]

---

### 📊 SCRIPT STATS

| Metric | Value |
|--------|-------|
| Total Words | [X] |
| Sentences | [X] |
| Avg Words/Sentence | [X] |
| Pause Points | [X] |
| Emphasis Words | [X] |
| Est. Duration | [X:XX] |

---

### 🔄 COPY-PASTE READY VERSION

**Plain text (no markers) for basic TTS:**
```
[Clean version without special markers]
```

**SSML Version (for advanced TTS):**
```xml
[SSML formatted version if tool supports]
```
```

---

## Tool-Specific Optimization

### ElevenLabs
- Supports natural speech patterns
- Use punctuation for pauses (no SSML needed)
- Commas = short pause, periods = longer pause
- Ellipsis (...) = thoughtful pause
- CAPS work for emphasis
- Supports emotional variation through settings

### PlayHT
- Supports SSML tags
- Use `<break time="Xs"/>` for precise pauses
- `<emphasis>` tags for stress
- `<prosody rate="X%">` for speed changes

### Murf AI
- Clean professional output
- Standard punctuation works well
- Supports style presets
- Good for consistent business tone

### Edge TTS (Free)
- SSML supported
- Use `<break/>` tags
- Limited emotion control
- Good for basic needs

### Google TTS
- Full SSML support
- `<break>`, `<emphasis>`, `<prosody>` tags
- Basic but reliable
- Good language support

---

## Pace Conversion Reference

| Pace | WPM | 100 Words = | 500 Words = |
|------|-----|-------------|-------------|
| Slow | 125 | 48 sec | 4:00 |
| Medium | 150 | 40 sec | 3:20 |
| Fast | 170 | 35 sec | 2:56 |
| Very Fast | 190 | 32 sec | 2:38 |

---

## Sentence Optimization Rules

### Original vs Optimized

**Too Long (Hard for TTS):**
```
"In this video, I'm going to show you the five most amazing AI tools
that will completely change how you work and make you ten times
more productive in less than a week."
```

**Optimized (Natural Speech):**
```
"In this video... I'll show you five amazing AI tools.
These will change how you work.
And make you ten times more productive... in less than a week."
```

### Guidelines
- Max 15-20 words per sentence
- One idea per sentence
- Add pauses after key points
- Break long lists with pauses

---

## Common Optimizations

### Numbers
| Original | Optimized |
|----------|-----------|
| 1000 | one thousand |
| 50% | fifty percent |
| $99.99 | ninety-nine dollars and ninety-nine cents |
| 10x | ten times |
| 2024 | twenty twenty-four |

### Abbreviations
| Original | Optimized |
|----------|-----------|
| AI | A.I. (or "artificial intelligence" first time) |
| CEO | C.E.O. |
| etc. | et cetera |
| vs | versus |
| w/ | with |

### Symbols
| Original | Optimized |
|----------|-----------|
| & | and |
| @ | at |
| + | plus |
| = | equals |

---

## Output Checklist

Before delivering voice script:
- [ ] Script broken into logical sections
- [ ] Pause markers added appropriately
- [ ] Emphasis words marked
- [ ] Pronunciation guides for difficult terms
- [ ] Numbers converted to spoken form
- [ ] Sentences optimized for speech length
- [ ] Tool-specific settings provided
- [ ] Copy-paste ready version included
- [ ] Duration estimate accurate
- [ ] Voice direction notes included

---

## Reference Files

| File | When to Read |
|------|--------------|
| `references/tts-tools.md` | Detailed tool settings and capabilities |
| `references/ssml-guide.md` | SSML tags and advanced formatting |
| `references/pronunciation-dictionary.md` | Common tech terms pronunciation |
