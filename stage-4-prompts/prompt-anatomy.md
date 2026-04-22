# 🎼 STAGE 4 — SUNO v5.5 PROMPT ENGINEERING

*The complete guide to writing prompts that generate usable Hindi indie songs.*

---

## ⚠️ BEFORE WE START: SUNO v5.5 REALITIES

Suno is powerful but unpredictable. Key truths:
- **Simple mode = lottery.** Always use Custom mode for control.
- **Lyrics box overrides style prompt** for arrangement. The prompt guides the production; lyrics guide the structure.
- **BPM in the prompt WORKS.** 75 BPM = immediately usable results for lo-fi.
- **Stacking specific sounds** (e.g., "Roland Juno pads") forces the AI to pull from better training data.
- **Hindi pronunciation is still a challenge.** We must account for this in how we write lyrics + guide vocal delivery.
- **First generation is rarely the best.** Plan for 3-5 iterations per song.
- **Regenerations save 80% of trouble.** If it's broken on first pass, refine and regenerate.

---

## 🧬 THE 5-LAYER PROMPT ANATOMY

Every Suno v5.5 prompt has 5 layers:

```
[STYLE] + [MOOD/VIBE] + [INSTRUMENTATION] + [VOCAL GUIDANCE] + [STRUCTURE]
```

Example:
```
Hindi indie lo-fi pop, warm melancholic evening mood, 
acoustic guitar and soft piano, male vocal, breathy and intimate, 
BPM 80, C major, 2:30 duration, heartfelt chorus-first structure
```

---

## 🎭 LAYER 1 — STYLE

**What it is:** The genre/genres that define the song's foundation.

### For Hindi Indie, these are our core styles:
- Hindi indie pop
- Desi lo-fi pop
- Acoustic Hindi folk-pop
- Hindi bedroom pop
- Indie rock (lighter)
- Hindi electronica / ambient
- Hinglish hip-hop / rap
- Bollywood-indie crossover

### Style stacking (what works):
- `"Hindi indie lo-fi pop"` ✓
- `"Acoustic Hindi folk-pop with modern production"` ✓
- `"Lo-fi hip hop with Hindi vocal"` ✓
- `"Hindi bedroom pop, raw and intimate"` ✓
- `"Indie electronic with Hindi vocals, cinematic"` ✓

### Style stacking (what fails):
- Just `"Hindi music"` ❌ (too vague)
- Just `"pop"` ❌ (no India context)
- `"Bollywood style"` ❌ (Suno defaults to old Bollywood, not indie)

### References (without copying):
We can reference artists for Suno's training data alignment:
- `"like early Prateek Kuhad"`
- `"like lighter Aditya Rikhari"`
- `"like mellow Armaan Malik indie"`

---

## 💭 LAYER 2 — MOOD/VIBE

**What it is:** One or two words about the emotional temperature + elaboration.

### Mood vocabulary for Hindi indie:
**High energy:**
- Upbeat, cheerful, celebratory, carefree, playful, euphoric

**Medium energy:**
- Warm, introspective, dreamy, contemplative, nostalgic

**Low energy:**
- Melancholic, introspective, bittersweet, intimate, quiet, raat ko

### What works:
- `"warm melancholic evening"` ✓
- `"bittersweet 2 AM introspection"` ✓
- `"intimate and yearning, like rain on a window"` ✓
- `"carefree but slightly sad underneath"` ✓

### The emotional layering trick:
**Two moods stacked = more interesting than one.**
- `"upbeat but lonely underneath"`
- `"celebratory but hollow"`
- `"dreamy but清醒"`

---

## 🎸 LAYER 3 — INSTRUMENTATION

**What it is:** What instruments carry the production, and what texture they create.

### Core Hindi Indie instrumentation:
| Instrument | Vibe | Works for |
|-----------|------|-----------|
| Acoustic guitar | Warm, folk, intimate | Heartbreak, self-worth, lo-fi |
| Electric guitar (clean) | Dreamy, indie rock | Travel, nostalgia |
| Piano / Keys | Emotional, cinematic | Heartbreak, late-night |
| Synth / Pad | Modern, dreamy | Party, independence |
| Lo-fi textures (vinyl crackle, rain) | Intimate, raat | Late-night, heartbreak |
| Minimal percussion | Raw, intimate | Lo-fi, folk |
| Full drum kit | Upbeat, party | Travel, freedom, party |

### What works in prompts:
- `"acoustic guitar and soft piano"` ✓
- `"lo-fi hip hop, vinyl crackle, rain sounds, 75 BPM"` ✓
- `"clean electric guitar, minimal drums"` ✓
- `"synth pad, warm bass, 110 BPM"` ✓

### The specific vs. vague rule:
**Specific instrumentation = higher quality output.**

❌ `"guitar and drums"`
✅ `"acoustic guitar fingerpicking, warm piano chords, light snare"`

### Production texture words:
- Raw, lo-fi, polished, cinematic, bedroom, intimate, warm, cold, dreamy, gritty

---

## 🎤 LAYER 4 — VOCAL GUIDANCE

**What it is:** Everything about the singing that affects how the lyrics land.

### Gender:
- Male
- Female  
- Duet (if two distinct parts)
- Multiple (group feel)

### Vocal tone words:
| Tone | Works for |
|------|-----------|
| Breathy | Late-night, heartbreak, intimate |
| Smooth | Romance, party, warm |
| Gritty | Independence, raw emotion |
| Powerful | Anthems, self-worth |
| Soft / Quiet | Intimate, lo-fi |
| Speech-near | Indie authenticity, raw |
| Urgent / Desperate | Emotional peaks, heartbreak |

### Hindi-specific guidance:
- `"clear Hindi pronunciation"` — MUST include this
- `"slight Hindi accent, intimate"` — for authenticity
- `"breathy Hindi vocals"` — for emotional songs
- `"strong Hindi vowels, emotional delivery"` — for powerful choruses

### Common mistake:
If you don't specify Hindi pronunciation, Suno sometimes defaults to awkward Hindi or poor pronunciation. Always add: `"clear Hindi pronunciation"`.

---

## 📐 LAYER 5 — STRUCTURE

**What it is:** Guidance on song length, arrangement, and hook placement.

### Key parameters:

**Duration:**
- `"2:30"` — Short and tight (ideal for Reels)
- `"2:45"` — Standard for streaming
- `"3:00"` — Risk of early skip

**Hook placement:**
- `"hook in first 30 seconds"` ✓
- `"chorus lands early"` ✓
- `"melodic intro before lyrics"` — tells Suno to ease in

**Structure:**
- `"verse-chorus-verse-chorus-bridge-chorus"` ✓
- `"open with chorus hook"` ✓
- `"no long intro, hook hits fast"` ✓

---

## 🔧 NEGATIVE PROMPTING (What to avoid)

Suno can be told what NOT to do. Add to any prompt:

```
Avoid: Auto-tune overuse, Bollywood clichés, generic pop, 
English-only lyrics when Hindi requested, awkward Hindi pronunciation
```

Or specify what's NOT in the song:
```
no Auto-Tune, no Bollywood orchestration, no heavy dhol drums
```

---

## 📝 PROMPT TEMPLATES

### Template 1: Heartbreak / Late Night
```
Hindi indie lo-fi pop, warm melancholic evening mood, 
acoustic guitar and soft piano, breathy male vocal, 
clear Hindi pronunciation, BPM 75, intimate bedroom production,
hook lands in first 30 seconds, 2:30 duration, bittersweet
```

### Template 2: Self-Worth / Independence
```
Hindi indie pop, confident but slightly introspective,
warm acoustic guitar and clean electric guitar,
male vocal, smooth but with grit, clear Hindi pronunciation,
BPM 95, anthemic chorus, hook hits early, 2:45 duration
```

### Template 3: Party / Freedom / Travel
```
Upbeat Hindi indie pop, carefree and euphoric,
acoustic guitar and synth, full drums, male vocal,
energetic delivery, BPM 115, C major, 2:30 duration,
no auto-tune, party anthem structure, hook in first 20 seconds
```

### Template 4: Monsoon Romance
```
Hindi indie bedroom pop, dreamy and nostalgic,
soft piano and acoustic guitar, rain texture,
female vocal, breathy and intimate, clear Hindi pronunciation,
BPM 80, romantic mood, 2:45 duration, emotional chorus
```

### Template 5: Lo-Fi Study / Chill
```
Lo-fi Hindi indie hip hop, introspective and calm,
vinyl crackle, rain sounds, soft piano,
breathy male vocal, BPM 75, 2:30, intimate production,
clear Hindi pronunciation, no drums, chill vibe
```

---

## 🔄 THE ITERATION WORKFLOW

### Every song gets v1 → v2 → v3 prompts:

**v1 (initial):** Run with the template + lyrics

**v2 (if needed):**
- Problem: Hook is weak
- Fix: Add `"strong melodic hook"` + specify hook placement earlier
- Problem: Hindi pronunciation bad
- Fix: Add `"very clear Hindi pronunciation"` + `"emphasize Hindi vowels"`
- Problem: Melody too generic
- Fix: Add `"memorable melodic hook, distinctive melody"`

**v3 (if needed):**
- Adjust BPM up/down
- Swap instrumentation (guitar → piano)
- Change vocal tone (breathy → powerful)

**Final:** Log the working prompt with what changed and why

---

## 🚨 SUNO v5.5 PRO TIPS

1. **BPM in prompt works:** `"75 BPM"` gives immediate usable results
2. **Stack specific sounds:** `"Roland Juno pads, gated snare reverb"` > `"synth"`.
3. **Simple mode is a lottery** — always Custom mode.
4. **Regenerate if Hindi is garbled** — it's a common failure mode
5. **Audio Influence slider:** For Custom mode, set to 0.3-0.5 to keep lyrics dominant
6. **Don't overwhelm the prompt** — 2-3 sentences is enough. More ≠ better.
7. **Test your prompt mentally:** Would a music producer understand it?

---

*Last Updated: 2026-04-22*
*Version: 1.0 (Seed — refine with each song)*