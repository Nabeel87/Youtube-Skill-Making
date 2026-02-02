---
name: script-writer
description: |
  Write engaging YouTube video scripts based on topic and preferences.
  This skill should be used when users say "write script", "create script",
  "script for", "video script", or "make script about".
---

# Script Writer

Create engaging, structured YouTube video scripts through guided MCQ questions.

## What This Skill Does

- Asks 6 MCQ questions to understand script requirements
- Generates complete video scripts with hooks, body, and CTA
- Provides word counts matching target video length
- Outputs copy-paste ready scripts

## What This Skill Does NOT Do

- Generate thumbnails (use `image-prompt-generator` skill)
- Create video prompts (use `video-prompt-generator` skill)
- Optimize for TTS (use `voice-script-generator` skill)

---

## Workflow

### Step 1: Ask MCQ Questions (One at a Time)

**IMPORTANT:** Ask one question → Wait for answer → Then next question

---

**Q1: Video Topic**
```
📝 What's your video topic/niche?

Type your topic OR select from common options:
A) AI Tools Review
B) Make Money Online
C) Tech Tutorial
D) Facts & Lists
E) Motivation
F) Gaming
G) Custom (type your topic)
```

---

**Q2: Video Length**
```
⏱️ Target video length?

A) Short (1-3 min) — ~300-500 words
B) Medium (5-8 min) — ~800-1200 words
C) Long (10-15 min) — ~1500-2200 words
D) Extended (20+ min) — ~3000+ words
```

---

**Q3: Video Format**
```
🎬 Video format/structure?

A) Listicle (5 Tips, 7 Tools, 10 Ways)
B) Tutorial (How to do X step by step)
C) Story-based (Problem → Solution → Result)
D) Comparison (X vs Y)
E) Explainer (What is X and why it matters)
F) Review (Product/Service review)
```

---

**Q4: Tone/Style**
```
🎭 Tone/style?

A) Professional & Authoritative
B) Casual & Friendly
C) Energetic & Hyped
D) Calm & Educational
E) Inspirational & Motivational
```

---

**Q5: Primary Goal**
```
🎯 Primary goal of this video?

A) Get subscribers (focus on CTA)
B) Drive traffic to website/link
C) Build authority/trust
D) Go viral (shareable content)
E) Educate audience
```

---

**Q6: Hook Style**
```
🪝 How do you want to start the video?

A) Question hook ("Have you ever wondered...")
B) Shocking statement ("This will change everything...")
C) Story hook ("Last week, something happened...")
D) Promise hook ("By the end of this video, you'll...")
E) Problem hook ("If you're struggling with X...")
```

---

### Step 2: Generate Script

After collecting answers, generate script using this structure:

---

## Script Structure Templates

### Listicle Format
```
[HOOK - 15-30 seconds]
[Question/Statement that grabs attention]
[Preview what they'll learn]
"Stay till the end for number X - it's the most powerful one"

[INTRO - 15-20 seconds]
Quick intro (if personal brand)
"Let's dive right in"

[ITEM 1]
- Name/Title of tip
- What it is (1-2 sentences)
- Why it matters
- Quick example or proof
- Transition to next

[ITEM 2-N]
(Same structure, increasing value)

[FINAL ITEM - Make it the best]
- Build anticipation
- Deliver the most valuable tip
- Explain why you saved it for last

[CTA - 20-30 seconds]
- Recap value delivered
- Clear call to action
- Engagement prompt (comment question)
- Subscribe reminder
```

### Tutorial Format
```
[HOOK - 15-30 seconds]
[Show the end result first]
"In the next X minutes, I'll show you exactly how to..."

[PROBLEM - 30 seconds]
- Acknowledge the struggle
- Show you understand their pain

[SOLUTION OVERVIEW - 30 seconds]
- Brief overview of what you'll teach
- Why this method works

[STEP 1]
- Clear instruction
- Show exactly what to do
- Common mistake to avoid

[STEP 2-N]
(Continue with clear steps)

[RECAP - 30 seconds]
- Quick summary of all steps
- Reinforce how easy it was

[CTA]
- What to do next
- Related video suggestion
- Subscribe prompt
```

### Story-Based Format
```
[HOOK - 20-30 seconds]
[Start in the middle of action/emotion]
"I was about to give up when..."

[SETUP - 1-2 minutes]
- Background context
- The problem/challenge faced
- Why it mattered

[JOURNEY - Main content]
- What you tried (failures)
- The turning point
- What actually worked

[TRANSFORMATION - 1 minute]
- The results
- Before vs After
- Proof/evidence

[LESSON - 1-2 minutes]
- What you learned
- How viewer can apply it
- Actionable takeaways

[CTA]
- Emotional connection
- Invite them to share their story
- Subscribe for more
```

### Comparison Format
```
[HOOK]
"X vs Y - which one is actually better? I tested both..."

[CRITERIA SETUP]
- What we're comparing
- The criteria/factors
- Why this matters

[OPTION A ANALYSIS]
- Pros (with evidence)
- Cons (be honest)
- Best for: [use case]

[OPTION B ANALYSIS]
- Pros (with evidence)
- Cons (be honest)
- Best for: [use case]

[VERDICT]
- Clear winner (or "it depends" with specifics)
- Quick recommendation based on viewer type

[CTA]
- Ask which they prefer
- Subscribe for more comparisons
```

---

## Output Template

Generate script in this exact format:

```markdown
## 🎬 Video Script

**Topic:** [Topic]
**Length:** [X minutes] (~[X] words)
**Format:** [Format type]
**Tone:** [Tone]

---

### 📌 TITLE OPTIONS
1. [Title option 1 - curiosity gap]
2. [Title option 2 - number + benefit]
3. [Title option 3 - how-to style]

---

### 🪝 HOOK (0:00 - 0:30)

[Write the exact hook script here]

---

### 📖 MAIN CONTENT

**[Section 1 Title]** (0:30 - X:XX)

[Full script for section 1]

**[Section 2 Title]** (X:XX - X:XX)

[Full script for section 2]

[Continue for all sections...]

---

### 🎯 CTA (Final 30 seconds)

[Write the exact CTA script]

---

### 📊 Script Stats
- **Total words:** [X]
- **Estimated length:** [X:XX]
- **Hook strength:** [X/10]
- **CTA clarity:** [X/10]

---

### 💡 Production Notes
- **B-roll suggestions:** [List 3-5 visual suggestions]
- **Text overlays:** [Key points to display on screen]
- **Music mood:** [Suggested music type]
```

---

## Tone Guidelines

| Tone | Language Style | Words to Use | Words to Avoid |
|------|---------------|--------------|----------------|
| Professional | Formal, data-driven | "research shows", "experts agree" | slang, "like", "you know" |
| Casual | Conversational | "honestly", "look", "here's the thing" | jargon, complex terms |
| Energetic | Punchy, excited | "insane", "game-changer", "let's go" | slow phrases, passive voice |
| Calm | Measured, clear | "let me explain", "consider this" | hype words, urgency |
| Motivational | Empowering | "you can", "imagine", "what if" | negative phrases, doubt |

---

## Word Count Guide

| Video Length | Words | Sections | Hook | CTA |
|--------------|-------|----------|------|-----|
| 1-3 min | 300-500 | 3-4 | 50 | 50 |
| 5-8 min | 800-1200 | 5-7 | 75 | 75 |
| 10-15 min | 1500-2200 | 7-10 | 100 | 100 |
| 20+ min | 3000+ | 10-15 | 150 | 150 |

---

## Output Checklist

Before delivering script:
- [ ] Hook grabs attention in first 5 seconds
- [ ] Word count matches target length
- [ ] Format matches selected structure
- [ ] Tone is consistent throughout
- [ ] CTA is clear and specific
- [ ] Title options are clickable
- [ ] Timestamps are included
- [ ] Production notes provided

---

## Reference Files

| File | When to Read |
|------|--------------|
| `references/hook-templates.md` | More hook examples by niche |
| `references/cta-templates.md` | High-converting CTA scripts |
