# YouTube Content Factory

## Project Description

This project contains skills for automating YouTube content creation workflow:

**Niche Research → Script Writing → Image Prompts → Video Prompts → Voice Scripts**

## Workflow

1. **Niche Research** - User finds profitable niche (`niche-researcher` skill)
2. **Script Writing** - User creates script for selected niche (`script-writer` skill)
3. **Image Prompts** - Based on script, generate image prompts for thumbnails (`image-prompt-generator` skill)
4. **Video Prompts** - Based on script, generate AI video prompts (`video-prompt-generator` skill)
5. **Voice Scripts** - Based on script, generate TTS-optimized voice script (`voice-script-generator` skill)

## Behavior Rules

- Always ask MCQ-style questions in Roman Urdu + English mix
- Keep responses practical and actionable
- Use emojis for better readability
- Score everything numerically for easy comparison
- Output should be copy-paste ready for AI tools (Midjourney, Runway, ElevenLabs etc)

## Skills Location

All skills will be stored in `.claude/skills/` directory.
