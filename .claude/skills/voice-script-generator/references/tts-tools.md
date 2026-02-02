# TTS Tool Specifications & Settings

## ElevenLabs

### Overview
| Spec | Value |
|------|-------|
| Quality | ⭐⭐⭐⭐⭐ Best natural quality |
| Price | Paid ($5-$22/month) |
| Languages | 29+ languages |
| Voice Cloning | Yes |
| Emotions | Yes (through settings) |
| SSML | Limited (punctuation-based) |

### Recommended Settings by Content Type

**YouTube Tutorial:**
```
Voice: Adam, Rachel, or Antoni
Stability: 0.50-0.65
Similarity: 0.75
Style: 0.30-0.45
Speed: 1.0
```

**Dramatic/Story:**
```
Voice: Daniel, Bella
Stability: 0.30-0.45
Similarity: 0.80
Style: 0.50-0.70
Speed: 0.95
```

**Professional/Business:**
```
Voice: Adam, Charlotte
Stability: 0.70-0.80
Similarity: 0.75
Style: 0.20-0.30
Speed: 1.0
```

**Energetic/Tech:**
```
Voice: Josh, Emily
Stability: 0.45-0.55
Similarity: 0.70
Style: 0.40-0.55
Speed: 1.05-1.10
```

### Best Voices by Type
| Type | Male | Female |
|------|------|--------|
| Professional | Adam | Charlotte |
| Friendly | Antoni | Rachel |
| Dramatic | Daniel | Bella |
| Energetic | Josh | Emily |
| Warm/Narrator | Clyde | Domi |

### Tips for ElevenLabs
1. Lower stability = more expressive, higher = more consistent
2. Use ellipsis (...) for dramatic pauses
3. CAPS for strong emphasis
4. Commas for natural breathing points
5. Keep sentences under 20 words for best results

---

## PlayHT

### Overview
| Spec | Value |
|------|-------|
| Quality | ⭐⭐⭐⭐ Great quality |
| Price | Paid ($29-$99/month) |
| Languages | 142+ languages |
| Voice Cloning | Yes |
| Emotions | Yes (emotion tags) |
| SSML | Full support |

### Recommended Settings

**Standard YouTube:**
```
Voice: Matthew, Joanna (US)
Speed: 1.0
Pitch: 0
Emotion: Neutral to Friendly
```

**Professional:**
```
Voice: Brian, Amy (UK)
Speed: 0.95
Pitch: 0
Emotion: Confident
```

### SSML Examples for PlayHT
```xml
<!-- Pause -->
<break time="500ms"/>

<!-- Emphasis -->
<emphasis level="strong">important</emphasis>

<!-- Speed change -->
<prosody rate="slow">Take your time</prosody>

<!-- Pitch change -->
<prosody pitch="+10%">Excited voice</prosody>
```

---

## Murf AI

### Overview
| Spec | Value |
|------|-------|
| Quality | ⭐⭐⭐⭐ Professional quality |
| Price | Paid ($23-$79/month) |
| Languages | 20+ languages |
| Voice Cloning | Limited |
| Emotions | Yes (style presets) |
| SSML | Partial |

### Best For
- Corporate/business content
- E-learning and training
- Professional presentations
- Clean, consistent output

### Recommended Voices
| Type | Voice |
|------|-------|
| Corporate Male | Marcus, Thomas |
| Corporate Female | Julia, Sarah |
| Casual Male | Miles, Ryan |
| Casual Female | Lily, Emma |

### Style Presets
- Conversational
- Newscast
- Assistant
- Promo
- Narration

---

## Edge TTS (Free)

### Overview
| Spec | Value |
|------|-------|
| Quality | ⭐⭐⭐ Decent quality |
| Price | FREE |
| Languages | 45+ languages |
| Voice Cloning | No |
| Emotions | Limited |
| SSML | Full support |

### Best Voices
| Language | Male | Female |
|----------|------|--------|
| US English | Guy | Jenny |
| UK English | Ryan | Sonia |
| Indian English | Prabhat | Neerja |
| Australian | William | Natasha |

### SSML for Edge TTS
```xml
<!-- Basic pause -->
<break time="1s"/>

<!-- Emphasis -->
<emphasis>keyword</emphasis>

<!-- Rate -->
<prosody rate="-10%">slower</prosody>
<prosody rate="+10%">faster</prosody>
```

### Command Line Usage
```bash
edge-tts --voice "en-US-JennyNeural" --file input.txt --write-media output.mp3
```

---

## Google TTS

### Overview
| Spec | Value |
|------|-------|
| Quality | ⭐⭐⭐ Basic but reliable |
| Price | Free tier available |
| Languages | 40+ languages |
| Voice Cloning | No |
| Emotions | Limited |
| SSML | Full support |

### Voice Types
- Standard - Basic quality
- WaveNet - Better quality
- Neural2 - Best quality

### SSML Support
```xml
<speak>
  Hello <break time="300ms"/> how are you?
  <emphasis level="strong">Important</emphasis>
  <prosody rate="slow" pitch="+2st">Dramatic</prosody>
</speak>
```

---

## Coqui TTS (Open Source)

### Overview
| Spec | Value |
|------|-------|
| Quality | ⭐⭐⭐ Variable |
| Price | FREE (open source) |
| Languages | Many |
| Voice Cloning | Yes |
| Emotions | Model dependent |
| SSML | Limited |

### Best For
- Developers
- Custom projects
- Privacy-focused use
- Experimentation

### Popular Models
- VITS - Fast, good quality
- YourTTS - Voice cloning
- Tacotron2 - Classic quality

---

## Quick Comparison

| Tool | Quality | Price | Emotions | SSML | Best For |
|------|---------|-------|----------|------|----------|
| ElevenLabs | ⭐⭐⭐⭐⭐ | $$$ | Yes | Basic | Premium YouTube |
| PlayHT | ⭐⭐⭐⭐ | $$ | Yes | Full | Professional |
| Murf | ⭐⭐⭐⭐ | $$ | Yes | Partial | Business |
| Edge TTS | ⭐⭐⭐ | Free | Limited | Full | Budget |
| Google TTS | ⭐⭐⭐ | Free+ | Limited | Full | Basic |
| Coqui | ⭐⭐⭐ | Free | Varies | Limited | Developers |

---

## Recommendation by Content Type

| Content | Best Tool | Reason |
|---------|-----------|--------|
| YouTube Long-form | ElevenLabs | Most natural |
| YouTube Shorts | Edge TTS | Quick, free |
| Business/Corporate | Murf | Professional |
| Podcast | ElevenLabs/PlayHT | Emotional range |
| E-learning | Murf | Consistent, clear |
| Experimentation | Coqui | Free, customizable |
