---
name: niche-researcher
description: |
  Find profitable YouTube niches through interactive MCQ questions.
  This skill should be used when users say "find niche", "niche research",
  "suggest niche", "topic ideas", or "what should I make videos about".
---

# Niche Researcher

Find the perfect YouTube niche through guided MCQ questions and scored recommendations.

## What This Skill Does

- Asks 6 MCQ questions one-by-one to understand preferences
- Scores niches based on user's priority and constraints
- Recommends top 3 niches with profitability analysis
- Provides actionable video ideas for each niche

## What This Skill Does NOT Do

- Write scripts (use `script-writer` skill)
- Generate thumbnails (use `image-prompt-generator` skill)
- Research specific keywords or SEO

---

## Workflow

### Step 1: Ask MCQ Questions (One at a Time)

**IMPORTANT:** Ask one question → Wait for answer → Then ask next question

---

**Q1: Content Category**
```
🎯 Select your content category:

A) Tech & AI Tools
B) Finance & Make Money Online
C) Health & Fitness
D) Gaming & Esports
E) Education & Tutorials
F) Facts & Entertainment
G) Motivation & Self-improvement
H) Cooking & Recipes
I) News & Current Affairs
J) Custom (type your own)
```

---

**Q2: Channel Type**
```
📹 What's your channel type?

A) Faceless (no face on camera)
B) Personal brand (face on camera)
C) Screen recording style
D) Mixed content
```

---

**Q3: Top Priority**
```
💰 What's your top priority?

A) High CPM (maximum earnings)
B) Easy to create
C) Viral potential
D) Evergreen content
E) Low competition
```

---

**Q4: Time Per Video**
```
⏰ How much time can you spend per video?

A) Under 2 hours
B) 2-5 hours
C) 5-10 hours
D) 10+ hours (quality focus)
```

---

**Q5: Target Audience**
```
🌍 Who is your target audience?

A) South Asia (Pakistan/India - Urdu/Hindi)
B) USA/UK (English speakers)
C) Global (mixed audience)
D) Middle East (Arabic)
```

---

**Q6: Channel Status**
```
📊 What's your current subscriber count?

A) 0-1K (new channel)
B) 1K-10K (growing)
C) 10K-100K (established)
D) 100K+ (large channel)
```

---

### Step 2: Calculate Niche Scores

After collecting all answers, use this scoring matrix:

| Niche | CPM | Ease | Viral | Evergreen | Competition |
|-------|-----|------|-------|-----------|-------------|
| AI Tools Reviews | 9 | 7 | 8 | 6 | 4 |
| Make Money Online | 10 | 5 | 7 | 7 | 3 |
| Personal Finance | 9 | 6 | 5 | 9 | 5 |
| Tech Tutorials | 7 | 6 | 6 | 8 | 5 |
| Gaming Clips | 4 | 9 | 9 | 4 | 3 |
| Facts & Lists | 5 | 8 | 8 | 7 | 4 |
| Motivation | 6 | 8 | 7 | 8 | 5 |
| Health Tips | 7 | 6 | 6 | 9 | 5 |
| Cooking | 5 | 7 | 6 | 9 | 6 |
| News Commentary | 6 | 7 | 8 | 3 | 5 |
| Crypto/Trading | 10 | 5 | 9 | 4 | 4 |
| Study Tips | 6 | 7 | 6 | 8 | 6 |

**Priority Weights:**
- High CPM: CPM×3, Ease×0.5, Viral×1, Evergreen×1, Competition×0.5
- Easy Content: CPM×0.5, Ease×3, Viral×1, Evergreen×1, Competition×0.5
- Viral: CPM×1, Ease×0.5, Viral×3, Evergreen×0.5, Competition×1
- Evergreen: CPM×1, Ease×1, Viral×0.5, Evergreen×3, Competition×0.5
- Low Competition: CPM×0.5, Ease×1, Viral×0.5, Evergreen×1, Competition×3

---

### Step 3: Generate Output

Use this exact template:

```markdown
## 🎯 Niche Analysis Results

### 📋 Your Profile
| Question | Your Answer |
|----------|-------------|
| Category | [Answer] |
| Channel Type | [Answer] |
| Priority | [Answer] |
| Time/Video | [Answer] |
| Audience | [Answer] |
| Subscribers | [Answer] |

---

### 🏆 Top 3 Recommended Niches

#### #1: [Niche Name] ⭐ Score: X/10

| Metric | Value |
|--------|-------|
| 💰 CPM Range | $X - $X |
| 📈 Growth Potential | X/10 |
| ⏰ Time Required | X hours/video |
| 🎯 Competition | Low/Medium/High |

**Why this fits you:** [2-3 sentences based on their answers]

**Video Ideas:**
1. [Specific video title idea]
2. [Specific video title idea]
3. [Specific video title idea]

---

#### #2: [Niche Name] ⭐ Score: X/10
[Same format]

---

#### #3: [Niche Name] ⭐ Score: X/10
[Same format]

---

### 📊 Quick Comparison

| Niche | CPM | Ease | Viral | Evergreen | **Overall** |
|-------|-----|------|-------|-----------|-------------|
| #1 | X/10 | X/10 | X/10 | X/10 | **X/10** |
| #2 | X/10 | X/10 | X/10 | X/10 | **X/10** |
| #3 | X/10 | X/10 | X/10 | X/10 | **X/10** |

---

### ✅ Next Steps

1. Pick your niche from the top 3
2. Use `/script-writer` to create your first script
3. Research 10 competitor channels in your niche
4. Plan your first 10 video titles
```

---

## Channel Type Compatibility

| Niche | Faceless | Personal Brand | Screen Recording | Mixed |
|-------|----------|----------------|------------------|-------|
| AI Tools | ✅ Best | ✅ Good | ✅ Best | ✅ Good |
| Make Money | ⚠️ OK | ✅ Best | ⚠️ OK | ✅ Good |
| Facts/Lists | ✅ Best | ⚠️ OK | ❌ Bad | ⚠️ OK |
| Gaming | ✅ Good | ✅ Good | ✅ Good | ✅ Best |
| Tutorials | ⚠️ OK | ✅ Good | ✅ Best | ✅ Good |
| Motivation | ✅ Best | ✅ Good | ❌ Bad | ⚠️ OK |
| Health | ❌ Bad | ✅ Best | ⚠️ OK | ✅ Good |
| Cooking | ❌ Bad | ✅ Best | ⚠️ OK | ✅ Good |

---

## Audience CPM Multipliers

| Audience | CPM Multiplier | Best Niches |
|----------|----------------|-------------|
| USA/UK | 1.0x (base) | Finance, Tech, Health |
| Global | 0.6x | Gaming, Tech, Entertainment |
| South Asia | 0.3x | Facts, Motivation, Cooking |
| Middle East | 0.5x | Business, Motivation |

---

## Output Checklist

Before delivering:
- [ ] All 6 questions answered
- [ ] Scores calculated with correct priority weights
- [ ] Top 3 niches match user's channel type
- [ ] CPM adjusted for target audience
- [ ] Video ideas are specific and actionable
- [ ] Next steps reference `/script-writer`

---

## Reference Files

| File | When to Read |
|------|--------------|
| `references/niche-database.md` | Detailed niche data and video ideas |
