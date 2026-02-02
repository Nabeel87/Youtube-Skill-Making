---
name: niche-researcher
description: |
  Helps YouTubers find profitable niches through interactive MCQ questions.
  This skill should be used when users say "find niche", "niche research",
  "suggest niche", "profitable niche", or want help choosing a YouTube niche.
---

# Niche Researcher

Find the perfect YouTube niche through guided MCQ questions and scored recommendations.

## What This Skill Does

- Asks 5 MCQ questions one-by-one to understand user preferences
- Scores and evaluates niche options based on answers
- Recommends top 3 niches with profitability scores
- Provides actionable next steps for chosen niche

## What This Skill Does NOT Do

- Create content or scripts (use `script-writer` skill)
- Generate thumbnails or images (use `image-prompt-generator` skill)
- Research specific keywords or SEO

---

## Workflow

### Step 1: Ask MCQ Questions (One by One)

Ask each question, wait for answer, then proceed to next.

**Q1: Content Category**
```
🎯 What's your main content category?

A) Tech & AI
B) Finance & Money
C) Health & Fitness
D) Gaming
E) Education & How-to
F) Entertainment & Lifestyle
G) Other (let me type)
```

**Q2: Target Audience Age**
```
👥 What's your target audience age?

A) 13-17 (Teens)
B) 18-24 (Young Adults)
C) 25-34 (Millennials)
D) 35-44 (Mid Adults)
E) 45+ (Mature)
```

**Q3: Channel Type**
```
📹 What type of channel do you have?

A) Faceless channel
B) Personal brand (face on camera)
C) Screen recording/tutorial
D) Mix of all
```

**Q4: Priority**
```
⭐ What's your priority?

A) High CPM (more money per view)
B) Easy content creation
C) Viral potential
D) Long-term evergreen content
E) Low competition
```

**Q5: Time Investment**
```
⏰ How much time can you spend per video?

A) 1-2 hours
B) 3-5 hours
C) Full day
D) Multiple days
```

---

### Step 2: Calculate Niche Scores

After collecting all answers, calculate scores using this matrix:

| Niche | CPM Score | Ease Score | Viral Score | Evergreen Score | Competition Score |
|-------|-----------|------------|-------------|-----------------|-------------------|
| AI Tools Reviews | 9 | 7 | 8 | 6 | 4 |
| Make Money Online | 10 | 5 | 7 | 7 | 3 |
| Personal Finance | 9 | 6 | 5 | 9 | 5 |
| Tech Tutorials | 7 | 6 | 6 | 8 | 5 |
| Gaming Clips | 4 | 9 | 9 | 4 | 3 |
| Facts & Lists | 5 | 8 | 8 | 7 | 4 |
| Motivation | 6 | 8 | 7 | 8 | 5 |
| Health Tips | 7 | 6 | 6 | 9 | 5 |
| Product Reviews | 8 | 5 | 5 | 7 | 4 |
| News Commentary | 6 | 7 | 8 | 3 | 5 |

**Scoring Formula:**
```
Final Score = (Category Match × 2) + (Priority Score × 3) + (Time Compatibility × 1.5) + (Channel Type Fit × 1.5)
```

---

### Step 3: Generate Output

Use this exact output template:

```markdown
## 🎯 Your Niche Analysis Results

### Your Profile Summary
- **Category:** [Selected]
- **Audience:** [Selected]
- **Channel Type:** [Selected]
- **Priority:** [Selected]
- **Time Available:** [Selected]

---

### 🏆 Top 3 Recommended Niches

#### #1: [Niche Name] ⭐ Score: X/10
- **CPM Range:** $X - $X
- **Why it fits you:** [Explanation based on answers]
- **Content ideas:** [3 video ideas]
- **Competition level:** Low/Medium/High

#### #2: [Niche Name] ⭐ Score: X/10
- **CPM Range:** $X - $X
- **Why it fits you:** [Explanation]
- **Content ideas:** [3 video ideas]
- **Competition level:** Low/Medium/High

#### #3: [Niche Name] ⭐ Score: X/10
- **CPM Range:** $X - $X
- **Why it fits you:** [Explanation]
- **Content ideas:** [3 video ideas]
- **Competition level:** Low/Medium/High

---

### 📊 Quick Comparison

| Niche | CPM | Ease | Viral | Evergreen | Overall |
|-------|-----|------|-------|-----------|---------|
| [#1]  | X/10 | X/10 | X/10 | X/10 | X/10 |
| [#2]  | X/10 | X/10 | X/10 | X/10 | X/10 |
| [#3]  | X/10 | X/10 | X/10 | X/10 | X/10 |

---

### ✅ Next Steps

1. **Pick your niche** from the top 3
2. **Use `/script-writer`** to create your first script
3. **Research 10 competitors** in your chosen niche
```

---

## Niche Database

### Tech & AI Niches
| Niche | CPM | Difficulty | Best For |
|-------|-----|------------|----------|
| AI Tools Reviews | $8-15 | Medium | Faceless, tutorials |
| Tech News | $6-12 | Easy | Commentary, news |
| Software Tutorials | $10-20 | Hard | Screen recording |
| Gadget Reviews | $8-15 | Medium | Personal brand |

### Finance Niches
| Niche | CPM | Difficulty | Best For |
|-------|-----|------------|----------|
| Make Money Online | $15-30 | Hard | Personal brand |
| Crypto/Trading | $12-25 | Medium | All types |
| Personal Finance | $10-20 | Medium | Tutorials |
| Side Hustles | $12-25 | Easy | Faceless |

### Entertainment Niches
| Niche | CPM | Difficulty | Best For |
|-------|-----|------------|----------|
| Facts & Lists | $3-8 | Easy | Faceless |
| Story Time | $4-10 | Medium | Personal brand |
| Reactions | $3-8 | Easy | Personal brand |
| Compilations | $2-6 | Easy | Faceless |

### Education Niches
| Niche | CPM | Difficulty | Best For |
|-------|-----|------------|----------|
| Language Learning | $8-15 | Medium | All types |
| Study Tips | $6-12 | Easy | Personal brand |
| Course Reviews | $10-18 | Medium | Screen recording |
| Skill Tutorials | $8-15 | Hard | Tutorial style |

---

## Output Checklist

Before delivering results:
- [ ] All 5 questions answered
- [ ] Scores calculated correctly
- [ ] Top 3 niches match user's priority
- [ ] CPM ranges are realistic
- [ ] Content ideas are specific and actionable
- [ ] Next steps include reference to other skills
