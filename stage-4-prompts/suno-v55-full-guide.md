# 🌊 STAGE 4 — SUNO v5.5 FULL GUIDE

*Operational knowledge for working with Suno v5.5 day-to-day.*

---

## 🎚️ HOW SUNO v5.5 WORKS

### Two generation modes:

**Simple Mode:**
- You give Suno a topic/style, it writes lyrics + generates music
- High variance, less control
- Useful for inspiration / "what if" exploration
- Not recommended for our pipeline

**Custom Mode:**
- You write your own lyrics (multi-stage, from Stage 3)
- You provide a style prompt (our 5-layer prompt)
- You control: duration, structure, instrumentation
- **This is our mode.** We need control.

### Key v5.5 Features:
- Better voice clarity than v3/v4
- Improved Hindi pronunciation (still imperfect — we guide it)
- Better arrangement control with custom lyrics
- Audio Influence slider: controls how much the style prompt dominates vs lyrics
- Duration control: 2:00-3:30

---

## ⚙️ CUSTOM MODE SETTINGS

### Recommended settings for Hindi Indie:
| Setting | Value | Why |
|---------|-------|-----|
| Mode | Custom | Full control |
| Duration | 2:30 | Reels-friendly, streaming optimal |
| Audio Influence | 0.3 - 0.5 | Keep lyrics dominant, let style guide production |
| Model | v5.5 | Latest |

### Audio Influence explained:
- **0.0-0.2:** Lyrics almost fully determine everything (melody, arrangement)
- **0.3-0.5:** Balanced — style has input but lyrics lead
- **0.6-1.0:** Style prompt dominates — changes melody and arrangement heavily

**For us:** 0.3-0.5 is the sweet spot. We write the lyrics; the style guides the production quality.

---

## ✍️ LYRICS INPUT GUIDE

### What to put in the lyrics box:
- **Multi-stage lyrics from Stage 3** — verses, chorus, bridge, outro
- **Section labels:** [Verse], [Chorus], [Bridge], [Outro]
- **Line breaks** within sections
- **No need to specify rhyme scheme** — Suno figures it out from the words

### Format example:
```
[Verse 1]
Tera saath tha lekin dil nahi tha
Itne kaar time bhidefine nahi kiya
Main apna khwab tha, tu sirf aaya

[Chorus]
Ab jaana hai, wapas nahi
Khud ko pehle main accha lagta hun
Tera intezaar, main nahi karta

[Verse 2]
Pehle tha tu, phir khaali raha
Ab khali mein bhi khushi hai
...

[Chorus]
...

[Outro]
...
```

### Tips:
- Don't write too many verses (2 max)
- Keep each section 4-8 lines
- The Chorus is the anchor — it must repeat
- Bridge is optional (not every song needs it)

---

## 🎯 SUNO SETTINGS FOR SPECIFIC SONG TYPES

### For Heartbreak Songs:
- Duration: 2:30
- BPM: 75-85
- Audio Influence: 0.3
- Key mood: melancholic, intimate

### For Party/Freedom Songs:
- Duration: 2:15-2:30
- BPM: 110-130
- Audio Influence: 0.4
- Key mood: upbeat, celebratory

### For Self-Worth Anthems:
- Duration: 2:45
- BPM: 90-105
- Audio Influence: 0.4
- Key mood: confident, warm

### For Lo-Fi / Late Night:
- Duration: 2:45
- BPM: 70-80
- Audio Influence: 0.2
- Key mood: intimate, lo-fi texture, vinyl crackle

---

## 🔄 REGENERATION STRATEGY

### When to regenerate:
| Problem | Fix |
|---------|-----|
| Hook is buried | Regenerate with earlier hook placement |
| Hindi pronunciation garbled | Regenerate — specify clear Hindi pronunciation again |
| Melody too generic | Regenerate with "memorable distinctive melody" |
| Production off | Regenerate with more specific instrumentation |
| Vocals sound Auto-Tuned | Regenerate with "no auto-tune, natural vocals" |
| Wrong mood | Regenerate with adjusted mood word |

### When NOT to regenerate:
- 90% of what you wanted is there, just minor tweak needed
- Take the audio into an editor instead
- Minor issues can be fixed in post, don't need full regen

---

## 📊 THE GENERATION LOG

Every song attempt gets logged:

```json
{
  "song_title": "Tera Intezaar",
  "date": "2026-04-22",
  "attempt_number": 1,
  "prompt_v": "v1",
  "bpm": 80,
  "duration": "2:30",
  "audio_influence": 0.3,
  "lyrics_summary": "Heartbreak, moving on",
  "scores": {
    "hook": 6,
    "melody": 7,
    "production": 7,
    "vocal": 5,
    "overall": 6
  },
  "notes": "Hindi pronunciation weak, hook lands well, melody good",
  "decision": "Regenerate — fix Hindi clarity"
}
```

---

## 🚨 COMMON FAILURES AND FIXES

| Failure | Likely Cause | Fix |
|---------|-------------|-----|
| Hindi words garbled | Suno struggles with Hindi phonetics | Write lyrics phonetically, add "clear Hindi pronunciation" |
| Hook never lands | Structure is too slow | Add "hook in first 20 seconds" |
| All songs sound same | Overusing same prompt template | Swap instrumentation, vary BPM |
| Vocals too Auto-Tuned | Default production style | Add "no auto-tune, natural vocals" |
| Melody is boring | Generic prompt | Add "memorable distinctive melody" |
| Wrong song length | No duration specified | Add exact duration in prompt |

---

*Last Updated: 2026-04-22*
*Version: 1.0*