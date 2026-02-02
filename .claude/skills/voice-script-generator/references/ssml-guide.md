# SSML (Speech Synthesis Markup Language) Guide

## What is SSML?

SSML is XML-based markup that gives you control over how TTS engines pronounce text.
Think of it as "formatting for speech" - like HTML but for audio.

---

## Basic Structure

```xml
<speak>
  Your text goes here with SSML tags for control.
</speak>
```

---

## Essential Tags

### 1. Break (Pause)

```xml
<!-- By time -->
<break time="500ms"/>   <!-- Half second -->
<break time="1s"/>      <!-- One second -->
<break time="2s"/>      <!-- Two seconds -->

<!-- By strength -->
<break strength="weak"/>     <!-- Small pause -->
<break strength="medium"/>   <!-- Normal pause -->
<break strength="strong"/>   <!-- Long pause -->
<break strength="x-strong"/> <!-- Very long pause -->
```

**When to use:**
- After important points
- Between sections
- For dramatic effect
- To let information sink in

---

### 2. Emphasis

```xml
<emphasis level="strong">very important</emphasis>
<emphasis level="moderate">somewhat important</emphasis>
<emphasis level="reduced">less important</emphasis>
```

**When to use:**
- Key terms
- Numbers you want highlighted
- Call-to-action words
- Brand names

---

### 3. Prosody (Speed, Pitch, Volume)

```xml
<!-- Speed -->
<prosody rate="slow">Take your time with this</prosody>
<prosody rate="medium">Normal speed</prosody>
<prosody rate="fast">Exciting fast part</prosody>
<prosody rate="75%">75% of normal speed</prosody>
<prosody rate="125%">125% of normal speed</prosody>

<!-- Pitch -->
<prosody pitch="low">Deep voice</prosody>
<prosody pitch="high">Higher voice</prosody>
<prosody pitch="+10%">Slightly higher</prosody>
<prosody pitch="-10%">Slightly lower</prosody>

<!-- Volume -->
<prosody volume="soft">Quiet part</prosody>
<prosody volume="loud">Loud part</prosody>
<prosody volume="+6dB">Louder</prosody>

<!-- Combined -->
<prosody rate="slow" pitch="low" volume="soft">
  Dramatic whisper
</prosody>
```

---

### 4. Say-As (Pronunciation Control)

```xml
<!-- Numbers -->
<say-as interpret-as="cardinal">123</say-as>      <!-- "one hundred twenty-three" -->
<say-as interpret-as="ordinal">1</say-as>         <!-- "first" -->
<say-as interpret-as="digits">123</say-as>        <!-- "one two three" -->

<!-- Dates -->
<say-as interpret-as="date" format="mdy">12/25/2024</say-as>  <!-- "December 25th, 2024" -->

<!-- Time -->
<say-as interpret-as="time">2:30pm</say-as>       <!-- "two thirty P M" -->

<!-- Currency -->
<say-as interpret-as="currency">$99.99</say-as>   <!-- "ninety-nine dollars and ninety-nine cents" -->

<!-- Spell out -->
<say-as interpret-as="spell-out">AI</say-as>      <!-- "A I" -->

<!-- Telephone -->
<say-as interpret-as="telephone">555-1234</say-as>  <!-- "five five five, one two three four" -->
```

---

### 5. Phoneme (Custom Pronunciation)

```xml
<!-- IPA alphabet -->
<phoneme alphabet="ipa" ph="ˈklaʊd">Claude</phoneme>

<!-- x-sampa alphabet -->
<phoneme alphabet="x-sampa" ph="klaUd">Claude</phoneme>
```

**Common use cases:**
- Brand names
- Foreign words
- Technical terms
- Names

---

### 6. Sub (Substitution)

```xml
<sub alias="World Wide Web Consortium">W3C</sub>
<sub alias="artificial intelligence">AI</sub>
<sub alias="doctor">Dr.</sub>
```

---

## Complete Examples

### YouTube Tutorial Intro

```xml
<speak>
  Hey everyone! <break time="300ms"/>

  Welcome back to the channel. <break time="500ms"/>

  Today, <break time="200ms"/>
  I'm going to show you <emphasis level="strong">five incredible</emphasis>
  AI tools <break time="300ms"/>
  that will <prosody rate="slow">completely change</prosody> how you work.

  <break time="800ms"/>

  And trust me, <break time="200ms"/>
  number <emphasis level="strong">five</emphasis>
  <break time="200ms"/>
  is <prosody pitch="+10%">absolutely game-changing</prosody>.

  <break time="500ms"/>

  So, <break time="200ms"/> let's dive in!
</speak>
```

### Professional Business Script

```xml
<speak>
  <prosody rate="95%">
    In today's competitive market, <break time="400ms"/>
    businesses need every advantage they can get.

    <break time="600ms"/>

    That's why <emphasis level="moderate">over 500 companies</emphasis>
    have already switched to our solution.

    <break time="500ms"/>

    <prosody pitch="-5%">
      The results speak for themselves.
    </prosody>

    <break time="400ms"/>

    <say-as interpret-as="cardinal">47</say-as> percent increase in productivity.
    <break time="300ms"/>
    <say-as interpret-as="cardinal">62</say-as> percent reduction in costs.
  </prosody>
</speak>
```

### Energetic Tech Review

```xml
<speak>
  <prosody rate="110%">
    <emphasis level="strong">Okay!</emphasis>
    <break time="200ms"/>

    This <break time="100ms"/> is <break time="100ms"/>
    <prosody pitch="+15%">INSANE!</prosody>

    <break time="400ms"/>

    The new <sub alias="M four">M4</sub> chip
    <break time="200ms"/>
    is <emphasis level="strong">blazing</emphasis> fast!

    <break time="300ms"/>

    We're talking <say-as interpret-as="cardinal">40</say-as> percent
    faster than last year's model!
  </prosody>
</speak>
```

---

## Tool Compatibility

| Tag | ElevenLabs | PlayHT | Edge TTS | Google TTS |
|-----|------------|--------|----------|------------|
| break | ✅ (via punctuation) | ✅ | ✅ | ✅ |
| emphasis | ❌ (use CAPS) | ✅ | ✅ | ✅ |
| prosody | ❌ | ✅ | ✅ | ✅ |
| say-as | ❌ | ✅ | ✅ | ✅ |
| phoneme | ❌ | ✅ | ✅ | ✅ |
| sub | ❌ | ✅ | ✅ | ✅ |

---

## Fallback for Non-SSML Tools

If using ElevenLabs or tools without SSML:

| SSML Effect | Fallback |
|-------------|----------|
| `<break time="500ms"/>` | Use `...` |
| `<break time="1s"/>` | Use `. ` (period + space) |
| `<emphasis>` | Use CAPS or *asterisks* |
| `<prosody rate="slow">` | Rewrite with shorter sentences |
| `<say-as>` | Write out the pronunciation |

---

## Best Practices

1. **Don't overuse** - Too many tags make speech unnatural
2. **Test iteratively** - Small changes, listen, adjust
3. **Match content** - Dramatic pauses for stories, minimal for tutorials
4. **Consider platform** - YouTube has auto-captions, clear speech helps
5. **Keep it readable** - Your script should still make sense without SSML
