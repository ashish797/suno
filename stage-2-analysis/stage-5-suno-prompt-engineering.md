# STAGE 5 — SUNO PROMPT ENGINEERING
## Synthesis: Turning Viral Data Into Suno v5.5 Prompts

---

## PART A: WHAT WE LEARNED FROM 20 SONGS

### Stage 1 — Title + Word + Plot
- **Title = Hook** in 60% of songs (single word, repetition-worthy)
- **Title syllable sweet spot:** 2-4 syllables
- **5 plot types dominate:**
  1. Heartbreak/longing (40%) — someone left, now what
  2. Longing/searching (30%) — wanting what's absent
  3. Devotion (15%) — possessive love
  4. Self-motivation (10%) — inner battle
  5. Moment-seizing (5%) — night decides
- **Concrete imagery over abstract** — tree, flower, path, eyes, breath
- "Kahan" (where) pattern: two of the biggest songs use searching questions

### Stage 2 — Structure
- **Hook lands in 30 seconds** (65% of songs)
- **Full 4-6 line chorus AS the hook unit** (60% of songs — NOT a short tagline)
- **Hook repeats 3-4× minimum** per song
- **Standard structure:** Verse → Chorus → Verse → Chorus → Bridge → Chorus
- **Runtime:** 3:00-3:30 (75% of songs)
- **End on hook, never on verse**

### Stage 3 — Lyrics
- **Hook syllable sweet spot:** 5-7 syllables (critical for Reels/short-form)
- **Rhyme scheme:** AA couplet dominates (45%)
- **Most reusable Hindi anchor phrases:**
  - "तेरे बिन" (without you) — GUL, TINKA pattern
  - "क्या कसूर है" (what sin) — KASOOR pattern
  - "क्या प्यार कम है" (is love less) — TERE HI HUM pattern
  - "तू कहाँ" (where are you) — TU KAHAN pattern
- **65% pure Hindi hooks** — Hinglish is exception, not rule
- **Body parts as imagery:** आँखें (eyes), ज़ुल्फ़ें (hair), दिल (heart), साँस (breath)

### Stage 4 — Production
- **BPM sweet spot:** 75-95 (50% of songs are 70-85)
- **4 mood clusters:**
  1. Late-night lo-fi (45%) — rain, city, intimate
  2. Melancholic acoustic (30%) — fingerpicked, confessional
  3. Rap-sung hybrid (15%) — male verse + female chorus
  4. Indie pop (10%) — slightly more produced
- **Instrumentation rules:**
  - ✅ Acoustic guitar dominant
  - ✅ Soft reverb on vocals
  - ✅ Minimal production — space matters
  - ❌ No tabla, dhol, Bollywood brass
  - ❌ No heavy auto-tune
  - ❌ Not overly produced

---

## PART B: SUNO v5.5 CUSTOM MODE — STRUCTURAL REQUIREMENTS

### What Must Be in Every Prompt

#### B1. Song Architecture
```
[Style/Genre] — [Mood] — [BPM guidance]
[Title: ___] — [Hook tagline ___ — single word hook: ___]
[Structure: Intro (8 bars) → Verse 1 → Chorus → Verse 2 → Chorus → Bridge → Chorus → Outro]
[Hook lands: first chorus, within 30 seconds]
[Runtime: 3:00-3:30]
[End on hook, do not end on verse]
```

#### B2. Vocal Instructions
```
[Voice: [male/female], [distance from mic: whisper-close/intimate/breath-weighted], [emotion: confessional/worn/urgent], [no auto-tune], [reverb on vocals]]
```

#### B3. Instrumentation
```
[Primary: [instrument]], [Secondary: [instrument]], [Percussion: [type]], [Production: [minimal/lo-fi/full arrangement]], [Avoid: [instruments/styles not wanted]]]
```

#### B4. Lyrics Quality Gates
```
[Hindi/Devanagari script] — [no pure English hook unless intentional] — [AA rhyme scheme minimum] — [hook: 5-7 syllables per tagline line]
```

---

## PART C: TEMPLATE PROMPT STRUCTURES

### Template 1: Late-Night Lo-Fi (Tu Kahan / Gul type)
```
Title: [TWO-SYLLABLE NOUN — singular, evocative]
Genre: Hindi indie lo-fi, late-night intimate
Mood: Melancholic warmth, first-person confession, urban solitude
BPM: 75-85

Structure:
- Intro: fingerpicked acoustic guitar alone, 4-8 bars, warm room reverb
- Verse 1: whisper-close vocals, minimal guitar, introspective
- Chorus: hook lands — full 4-line chorus, voice raw, guitar fills gently, soft percussion enters
- Verse 2: slightly warmer arrangement, intimacy deepens
- Chorus 2: identical lyrics, slightly fuller production
- Bridge: most stripped section — guitar + vocal only OR her voice enters
- Chorus 3: final — stripped arrangement, voice thinnnest, then full arrangement returns gently
- Outro: voice alone + one guitar note, fades or cuts

Vocal: Male voice, whisper-close, breath-heavy, slightly cracked on emotional words, intimate NOT loud, no auto-tune, reverb on vocals
Primary Instrument: Fingerpicked acoustic guitar, warm room reverb
Secondary: Soft piano chords underneath, warm bass line
Percussion: Soft brush drums on 2 and 4 only, whisper-soft
Production: Lo-fi, minimal, warm room acoustics, reverb-heavy vocals, lots of space
Avoid: Bollywood orchestration, tabla, dhol, heavy drums, auto-tune, over-production

Lyrics guidance: Pure Hindi, Devanagari. Hook tagline: 5-7 syllables. AA rhyme scheme. Body imagery (eyes, breath, hair). "तेरे बिन" or "तू कहाँ" anchor pattern.
```

### Template 2: Melancholic Acoustic (Kasoor / KGHK type)
```
Title: [SINGLE NOUN or QUESTION PHRASE — 2-4 syllables]
Genre: Hindi acoustic indie, confessional
Mood: Guilt, longing, emotional questioning, first-person admission
BPM: 75-85

Structure:
- Intro: acoustic guitar alone, simple repeating motif, 4 bars
- Verse 1: voice close-mic'd, guitar plays underneath, observational
- Pre-chorus: builds slightly, guitar intensifies
- Chorus: hook — full 4-line chorus, emotional peak, full arrangement
- Verse 2: complication — truth gets harder to say
- Chorus 2: repeat, slightly heavier
- Bridge: self-revelation, stripped or heightened
- Chorus 3: final — everything returns, emotional peak

Vocal: Male voice, intimate confessional, slight breathiness, not performed, raw
Primary Instrument: Fingerpicked acoustic guitar, clean tone
Secondary: Subtle strings on emotional moments only
Production: Clean, minimalist, confessional booth aesthetic, reverb on vocal
Avoid: Heavy production, drums louder than vocals, auto-tune, tabla/dhol

Lyrics guidance: Pure Hindi. Hook: 5-7 syllables. Question format "क्या..." works well. Sensory imagery pairs (eyes/hair, breath/lips). AA rhyme scheme.
```

### Template 3: Rap-Sung Hybrid (Dooriyan / Nidarr type)
```
Title: [SINGLE WORD or SHORT PHRASE — repetition-worthy, 2-4 syllables]
Genre: Hindi rap-sung ballad, urban emotional
Mood: First-person accountability, inner battle, surrender OR empowerment
BPM: 85-100 (rap sections), hooks can be slower

Structure:
- Intro: beat/ambient, establishes mood, 4 bars
- Verse 1: Male rap — first person, observational, trap hi-hats
- Pre-chorus: build — female voice enters subtly
- Chorus: Female singing voice — hook, contrast with male verse, emotional
- Verse 2: Male rap — deepens the story
- Chorus 2: Female chorus repeat, slightly fuller
- Bridge: key self-revelation (mother's voice OR internal truth)
- Chorus 3: Final — full arrangement, hook at emotional peak

Vocal: Male rap verse (flow, cadence), female singing chorus (melodic, warm, NOT auto-tuned)
Primary Instrument: Trap hi-hats + 808s OR acoustic guitar + trap mix
Secondary: Electric guitar layers (Nidarr/UNSTOPPABLE style)
Female Chorus: Warm, emotionally open, contrasts with male rap
Avoid: Female voice doing rap parts, male voice on hook (hook should be the "other" voice)

Lyrics guidance: Hinglish acceptable for rap sections, pure Hindi for hook. Hook: 5-7 syllables, full chorus as hook unit. AA rhyme. Male verse: more words, narrative. Female chorus: short, punchy, emotional.
```

### Template 4: Devotional / Possessive (Tere Hi Hum / Khat type)
```
Title: [POSSESSIVE PHRASE — "तेरे ___" pattern — 2-4 syllables]
Genre: Hindi indie acoustic, devotional intimacy
Mood: Absolute surrender, claiming the other, devotional love
BPM: 70-80

Structure:
- Intro: acoustic guitar, warm, 4 bars
- Verse 1: intimate address, confessing
- Chorus: hook — "तेरे ही हम" type construction, devotional
- Verse 2: escalating claims ("I'll do X for you")
- Chorus 2: repeat
- Bridge: devotional escalation ("tu hi khuda" type)
- Chorus 3: final

Vocal: Male voice, intimate, not loud, slightly higher register on devotional lines
Primary Instrument: Acoustic guitar, warm tone
Production: Minimal, intimate, reverb-heavy
Avoid: Bollywood devotional orchestration, heavy arrangements

Lyrics guidance: Pure Hindi. Possessive construction "तेरे बिन" / "तेरे ही" / "तू ही". Devotional paradox ("khuda mein maanu but dua maangu"). 5-7 syllable hook. AA rhyme.
```

---

## PART D: REFERENCE TRACK RECOMMENDATIONS

### By Mood Cluster

**Late-Night Lo-Fi:**
- Anuv Jain — HUSN, JO TUM MERE HO
- Aditya Rikhari — TU KAHAN, TINKA
- Prateek Kuhad — cold/mess, Kuch Din
- AUR — Tu Hai Kahan

**Melancholic Acoustic:**
- Prateek Kuhad — KASOOR, KHO GAYE HUM KAHAN, TERE HI HUM
- Anuv Jain — ALAG AASMAAN

**Rap-Sung Hybrid:**
- Dino James — DOORIYAN ft. Kaprila, NIDARR
- Dino James — UNSTOPPABLE ft. Deepna Kumar

**Devotional Intimate:**
- Navjyot Ahuja — KHAT
- Prateek Kuhad — TERE HI HUM

---

## PART E: SUNO v5.5 FULL PROMPT ANATOMY

### The Complete Prompt Structure (All Sections Together)

```
[INTRO: instrument + character + duration]

[VERSE 1: vocal style + lyrical subject + instrumental feel]

[PRE-CHORUS: optional, build feel]

[CHORUS: full hook section, how it sounds + exact lyrical note]

[VERSE 2: what changes, emotional progression]

[CHORUS 2: production change from Chorus 1]

[BRIDGE: what happens here, most stripped OR most heightened]

[CHORUS 3: final, emotional peak, production]

[OUTRO: how it ends]

[VOICE: detailed vocal notes]
[INSTRUMENTS: specific + general avoidance]
[PRODUCTION: overall character]
[LYRICS: language + structure rules]
[BPM: safe range]
[REFERENCE TRACKS: specific songs]
```

---

## PART F: COMMON SUNO MISTAKES TO AVOID

1. **Too much structure detail** — Suno can't follow complex arrangements. Keep structure broad.
2. **No lyric guidance** — Sans lyric mode produces generic. Always provide lyric direction in Hindi.
3. **BPM too fast** — anything over 110 starts losing the lo-fi intimate character
4. **"Full band"** — this triggers Bollywood. Say "minimal production" instead.
5. **Auto-tune mention** — kills the confessional authenticity. Don't ask for it.
6. **Generic Hindi** — say "pure Hindi Devanagari, 5-7 syllable hook, AA rhyme scheme"
7. **Hook too long** — tagline portion of hook must be 5-7 syllables. Full chorus can be longer.
8. **No verse/chorus separation in prompt** — Suno needs to know where sections break

---

## PART G: MASTER SONG — PRODUCTION GUIDE (next file)

See: `stage-2-analysis/master-song-production-guide.md`

This is the ONE fully detailed production guide — built from scratch using all Stage 1-4 learnings. Original Hindi lyrics, line-by-line production notes, exact instrumentation, vocal direction, and Suno prompt. All grounded in the 20-song dataset patterns.