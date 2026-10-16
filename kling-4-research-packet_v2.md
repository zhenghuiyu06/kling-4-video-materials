# Kling 4.0 Can Generate 30 Seconds. Can It Tell a Story?
## Research packet v2 (research only)

Updated 2026-10-16, about 10:40 Taipei. This packet analyses other creators' tests; none of the footage is ours. v2 adds a wider search for tests posted since full launch (2026-10-15 23:00 Taipei), Oprelia's on-screen prompts, TechHalla's prompt cards, a located E14, and re-checked Oprelia quotes. Section 11 lists every change from v1.

## 0. Bottom line

- **New first-hand full-model tests since launch.** YouTube adds two (Paul Donis / The AI Filmmaking Advantage; AI产品狙击手 kzhu). X adds four (Dheepanratnam, Dani__oros, HeyZoyaKhan, Starjupi). Bilibili, Douyin, Xiaohongshu and Reddit were blocked or turned up nothing locatable.
- **Revised YouTube counts:** A = 1, B = 5, C = 5, D = 12. Flash-only tests (excluded) = 23.
- **The biggest correction is TechHalla.** His prompt cards show that his "everyone stays on-model across every cut" clips were **7–8 second** generations at 1080p, not 30-second ones.
- **The closest thing to a fair test is Paul Donis's 11-test video.** He used the same prompt and inputs for each model and showed first takes only. Native resolutions differ and everything was upscaled, there is one sample per model, and he gives no verdict. So it is still not a controlled measurement.
- **Realistic length:** about 7 minutes of distinct, attributable test material. A ~10-minute video works if about 3 minutes are clearly labelled non-test segments: the official spec explained as claims, Flash vs full, a decision framework, and attributed comments. Going past 10 minutes would repeat material.
- **Permission:** none granted for any excerpt. Every YouTube item, new ones included, has the standard license; the yt-dlp `license` field is empty, so there is no Creative Commons flag.

## 1. Method (truthful access)

**Searches**
- YouTube: 12 date-sorted query variants, in English, Chinese, Spanish, Portuguese, Korean and Japanese, giving 212 results and 114 not seen in v1. Metadata was pulled for 25 new candidates.
- X: API search from 2026-10-15 15:00 UTC for posts with video, then the creators' threads.
- Bilibili: the search API returned an error page. Xiaohongshu redirects to a login page. Douyin is a JavaScript app that curl can't read. Reddit returned HTTP 403.
- Web search turned up one Chinese blog "实测" (a hands-on test write-up) on Juejin. It was published before launch and mostly restates official examples, so it is listed but not counted.

**How material was reviewed**
- Temporary low-resolution downloads were used for frame contact sheets: Oprelia (360p was the only format offered), Paul Donis, kzhu, AIFC, Eren, the TechHalla film, and 7 X videos.
- Audio was transcribed locally (faster-whisper small and small.en). That covers the Oprelia quote segments, Donis, kzhu, AIFC and Dheepanratnam.
- No video was watched end to end. No clips were cut. No footage is in the deliverables. All temporary files are deleted after this packet.

**How full 4.0 (not Flash) was confirmed:** on-screen model label or keyframe UI, then duration over 20s or 1080p, then a creator claim. Flash is limited to 20s, 720p and first frame only.

## 2. Counts (YouTube deduplicated; X and Reddit separate)

| Category | v1 | v2 | Items |
|---|---|---|---|
| A | 1 | **1** | Oprelia AI |
| B | 3 | **5** | Matt Starky; AiHustleGame (full vs Flash unconfirmed); TechHalla (now confirmed via 1080p in his prompt cards); **Paul Donis ZGelYMAihxQ (new)**; **kzhu gG0oCdvnADU (new, Chinese)** |
| C | 5 | **5** | Unchanged |
| D | 10 | **12** | + AIFC q8tB9zrByqc (Chinese partner film, pre-launch); + Eren Şerefoğlu yNvj7a1u8No (contest) |
| Flash-only (excluded) | 20 | **23** | + MOKSTORY c5vn2D74wOU; 妖精アーヤさん SbRna_uB9aI; ai_jinhyeong TMdgRPQCJc4 (descriptions say Flash) |
| Commentary on official demos / news (not tests) | 9 | **16** | + k2lvH3m13xA, 1kg2wpJ3BxM ("Not tested by me yet"), D5laFpOsSfQ, iW-dQJVtyD4, EcLhb24T2kE, BCbpbCMpLrg, pC_Pv25zbHU (unverified, metadata only) |
| X first-hand test posts | 4 | **8** | + Dheepanratnam, Dani__oros, HeyZoyaKhan, Starjupi. OpreliaAI's and iampauldonis's posts are deduplicated into M1 and M5. SilentNightX97 (15s) and shishirdotai (9s) are listed but unconfirmed. |
| Reddit | 1 snippet | **1 snippet** | No new posts found |

First-hand full-model tests that show process or prompts: **6 YouTube and 8 X.** That is still far below 30.

## 3. Spec facts (official)

- **Full Kling 4.0:** 3–30s; up to 10 image keyframes plus first/last frames; Omni Reference up to 15 assets; 720p, 1080p or 4K.
  - Kling's Oct 15 post lists 10-bit HDR and the API as "coming soon". Video extension to 2 minutes is also coming soon (user guide https://kling.ai/quickstart/kling-4-model-user-guide; feature page https://kling.ai/feature/kling-4-ai-video-generation; launch post https://x.com/Kling_ai/status/2110747537187709424).
- **Flash:** 3–20s, 720p, first frame only, no keyframes, available since 2026-09-28.
- **Credit cost:** not published. Matt Starky's panel at about 4:00 shows "840" on the Generate button with no unit label.

## 4. (A) Manifest

### 4.1 First-hand full-model tests

**M1. Oprelia AI, https://www.youtube.com/watch?v=GB0zuXi3SMU (2026-10-15, 23:53). Category A.**
- **Confirmed on screen.** Every test's details panel reads "Video · Kling 4.0", followed by aspect ratio and resolution. At about 19:25 the generation bar shows "Kling 4.0", Keyframes mode, and First / Middle / Last frame slots.
- **Prompts on screen, transcribed from 360p frames.** First lines only; the full texts are long. Times are approximate.

| Approx. time | Prompt opening (verbatim where legible) | Panel settings |
|---|---|---|
| ~8:00 | "SHOT 1 (00:00–00:01) — God's Eye Vertigo Drop…" (multi-shot timed prompt) | Kling 4.0 · Adaptive · 720p |
| ~8:30–9:50 | "Style: Photorealistic live-action surrealism… All characters are anthropomorphic animals…" subway scene, 4 references | Kling 4.0 · 16:9 · 720p |
| ~10:00–11:00 | "12-second video, 9:16. Use @image1 as the character reference… from the depth-map video @Video1…" | Kling 4.0 · 9:16 · 720p |
| ~11:30–12:30 | "20-second cinematic live-action scene, 16:9. Two adults stand outside a locked hotel room…" timed dialogue | Kling 4.0 · 16:9 · 720p |
| ~13:00 | "15-second 2D anime scene, 16:9. Use @image1 as the character design…" | Kling 4.0 · 16:9 · 720p |
| ~13:30 | "15-second 2D anime hand-to-hand fight, 16:9. Fighter A… Fighter B…" | Kling 4.0 · 16:9 · 720p |
| ~14:30 | "14-second Pixar-style 3D animated comedy, 16:9…" (roller-coaster couple; this is the clipped-dialogue clip) | Kling 4.0 · 16:9 · 720p |
| ~15:30 | "10-second action sequence, 16:9. Use @image1 as the girl's character…" (katana, training dummy) | Kling 4.0 · 16:9 · 720p |
| ~16:00 | "A photorealistic 14 second rooftop fight set in London… Buckingham Palace…" | Kling 4.0 · 16:9 · 720p |
| ~17:00–18:00 | "VOICE REFERENCE @1 defines Veyr's speaking voice… 14-second photorealistic dark fantasy scene…" | Kling 4.0 · 16:9 · 720p |
| ~18:30 | "A photorealistic 20 second rooftop fight…" (second attempt) | Kling 4.0 · 16:9 · 720p |
| ~20:30 | "One continuous photorealistic shot with a locked camera. A museum conservator reaches toward an antique brass clockwork bird…" (bird keyframe test) | Kling 4.0 · Adaptive · **1080p** |
| ~21:00–22:00 | "19-second photorealistic cinematic science-fiction fight sequence. Use the seven supplied images as key visual anchors…" (alien boxing, keyframes) | Kling 4.0 · Adaptive · 720p |

- **Full alien-boxing prompt** is posted by the creator at https://t.me/TheProPrompts/352, linked from https://x.com/OpreliaAI/status/2110832681114312973. Inputs: "First/last frame + multikey frames", 19 seconds. The X video is 19.1s.
- **Takeaway:** none of Oprelia's tests used 30 seconds. The longest were 20s.
- **Quotes re-checked** with a second, larger transcription model. Times are video timestamps.
  - 9:43–9:50: "this is not that bad in terms of like the look of it, but in terms of following the instructions, it's kind of off."
  - 14:37–14:49: "it cuts out, he was supposed to say 'not what I meant'… maybe because it was 14 seconds and it didn't have time to add all those audio in." This is the creator's guess at the cause.
  - 16:18: "the moment they do fast movements, it starts to break apart."
  - 16:35–16:42: "these cuts where they throw him down, it changes the position, the composition is wrong."
  - 17:03: "where it strives is realism."
  - 17:46: "pretty good audio cloning here."
  - 18:20–18:49: "even after a couple of tries on this, and this was another one that I deleted… these fighting sequences are not the strong point of Kling."
  - 19:00–19:08: "the characters' positions change suddenly, she's at the edge… that doesn't make any sense."
  - 20:01–20:05 (bird test): "this is bad because it doesn't show different camera angles."
  - 20:22–20:28: "the start is totally [expletive] up because it's actually missing… one middle frame."
  - 20:32: "this gives you the most amount of control right now over the model."
  - 20:42–20:52: "maybe you can do the fight sequences if you are going to be using these multi-keyframe [techniques]… this is by far the best video out of the bunch."
- **What changed from v1:** the keyframed fight was Oprelia's best result. The "fights break" verdict applies to fights generated without keyframes.
- **Permission:** standard license, needed.

**M2. Matt Starky, https://www.youtube.com/watch?v=pCGQjBk5vrE (2026-09-28). Category B.** Unchanged from v1.
- On screen at about 4:00: "VIDEO 4.0 Preview · 1080p · 30s · 9:16".
- Claim at 0:51–1:05: one generation is "a full UGC ad". Output at about 4:14 onward.
- Failures unknown. The transcript is unusable after about 2:00. Permission needed.

**M3. AiHustleGame, https://www.youtube.com/watch?v=QKBwA8VWMAY (2026-10-04). Category B.** Unchanged.
- Generated 10s shots, regenerated "if the character changes" (4:28), trimmed and cut in Premiere (4:38–5:20).
- Full vs Flash unconfirmed. Kling partner. Permission needed.

**M4. TechHalla, https://www.youtube.com/watch?v=9R7JL4HS4e0 (2026-10-15, 6:56) and X thread https://x.com/techhalla/status/2110806819937378773. Category B.**
- **Confirmed** by the creator's prompt cards, which state 1080p. That rules out Flash, though it is still the creator's own graphic.
- Card 01, Dynamic Motions: "OMNI REFERENCE · 16:9 · 7 s · 1080p · NATIVE AUDIO", 3 references, "1 prompt → 5 hard cuts in 7 seconds". The prompt is a timed beat list (0–2s, 2–3.5s, 3.5–5s, 5–6s, 6–7s) with "hard cut" markers.
- Card 02, Camera work: "8 s · 1080p", 3 references, 4 timed beats.
- Card 03, Omni Reference: "8 s · 1080p", 6 references, 5 timed beats, "Each of the four heroes appears only once; never duplicate anyone."
- **Correction:** the headline consistency claim refers to an **8-second** generation, not 30 seconds.
- **E14 located** in the film. The X copy and the YouTube copy are both 416s and the chapters match; the YouTube timestamps are inferred from that match.
  - Card 01 ≈ **2:52–3:00**, in the Laboratory chapter. The jungle run on screen is longer than the 1s prompt beat, so editing may have extended it (unknown).
  - Card 03 ≈ **5:40–5:48**.
  - Card 02 ≈ **6:09–6:15**, just before the "Final Stage · The Coast Road" title at 6:16.
- Failures: none disclosed. Permission needed.

**M5 (NEW). Paul Donis / The AI Filmmaking Advantage, "Can Kling 4.0 Beat Seedance 2.5? Same Prompt, First Takes, 11 Tests", https://www.youtube.com/watch?v=ZGelYMAihxQ. Category B.**
- Published 2026-10-16 05:56 Taipei, 6:22 long. The creator states he is a Kling AI Creative Partner.
- **Confirmed:** each Kling clip is labelled "KLING 4.0" on screen. The description says Kling ran at 1080p, and two Blender-guided runs were 24–27s. Both rule out Flash.
- **Method (creator's description):** "same prompt and the same inputs for every model, first takes only. No rerolls, no cherry-picking, no commentary." Native resolutions differ (Kling 1080p, Seedance 720p or 480p, MiniMax 2K), and every clip was upscaled to 4K with Topaz. The Seedance Confession take is labelled "POSTED SEPT 2026" while the Kling take is "TESTED OCT 2026", so the runs were made at different times. There is one sample per model and no verdict, so this is **not a controlled measurement**.
- **Timestamps (chapters):**
  - 0:05 building explosion; 0:35 warrior/troll; 1:05 pose.
  - 1:34 "Retro Blondie vs the robot army (Blender-guided)". Kling card reads "BLENDER-GUIDED · 27 s" with a start frame.
  - 2:28 robots; 2:58 samurai run; 3:28 car.
  - 4:03 "The Confession". Seedance is shown first; Kling ≈ **4:27–4:51**, labelled "1ST TAKE · NO REROLLS · 24 s · TESTED OCT 2026". The 5-shot interrogation prompt ends with "Matched eyelines across reverse angles; the two stay on the same axis."
  - 4:51 Kraken; 5:21 anime.
  - 5:51 "The Fridge" sitcom, 10s, Kling first (≈ 5:51–6:01).
- **Prompts:** shown on screen under every clip. They are too small at 360p to transcribe in full, so the full texts are **unknown**; the Confession prompt was partly legible.
- **What the sampled frames show** in the Kling Confession: two consistent characters across wide and reverse-angle singles. Whether the eyelines actually match was **not assessed**. No commentary or verdict from the creator.
- An X companion post (https://x.com/iampauldonis/status/2110863211981378029) re-posts the Robot Army test with its prompt visible. His thread opener (https://x.com/iampauldonis/status/2110858615414194675) reads: "AI video in 2027 is looking bleak… If nobody closes the gap, there's no reason for ByteDance to hurry."
- **Permission:** standard license, needed.

**M6 (NEW). AI产品狙击手 kzhu, "可灵4 0测评报告！六维鹈鹕骑车实测！" ("Kling 4.0 review: six-dimension pelican-on-a-bike test"), https://www.youtube.com/watch?v=gG0oCdvnADU. Category B. Mandarin.**
- Published 2026-10-16 09:50 Taipei, 2:09 long.
- **Confirmation:** creator claim only. He calls it Kling's newest release and posted after launch. Duration and settings are unknown, so Flash cannot be ruled out from evidence. Rated **creator-claimed**.
- **Timestamps:** prompt shown on screen 0:10–0:13; evaluation by dimension 0:24–1:56; closing 1:56–2:05.
- **Failures listed** in the voice-over (0:29–1:10) and the description:
  - an extra wall clock appears;
  - the bicycle's full structure is never visible;
  - the left wing doesn't hold the handlebar;
  - a glass bottle floats unsupported;
  - the mirror wall doesn't reflect;
  - the selfie uses the front camera instead of the rear;
  - the camera angle is off.
- **Successes:** the Chinese text "鹈鹕" (pelican) renders correctly, but the 3:45 clock is wrong (description).
- This is a single benchmark prompt the creator reuses across models (score page https://www.techgogogo.com/ai-video-benchmark/), so it is not controlled across models.
- **Permission:** standard license, needed.

### 4.2 Official (C)
Unchanged: nlM7kL3kv_Y, w3397LF5MAc, EteSu9OCWMg (mixes 4.0 and Flash), b9lEL1hClRg (Simon Meyer: "50 times on this one shot", 2:14; "in like 80% of the shots the lip sync was really, really good", 2:38), YuxI05lHLRk. Never present these as independent tests.

### 4.3 Output-only (D)
Process and settings are unknown for all of these. Permission is needed for each.
- **v1 items (10), unchanged:** SPARE b2jR0rOGEKQ; Artem Brinn wvwhG8m7Bf0; Dave Clark BYYy4wLRK6c (mixed with Seedance); Alex Patrascu fpxqbVki7M4; soegimitro uk4ls1cWvxY; Immagina Z_uE3cu3XRg; AiBite LT97uVbMT6E; ysf.ai mG1SlgBVeqk; Eren Şerefoğlu HTQoJUjqeE0; Ady DeeJay 3WtuJpwfGZY.
- **New: AIFC · AI FILM COLLECTIVE,** https://www.youtube.com/watch?v=q8tB9zrByqc (2026-09-30 03:44 Taipei, 5:48). Pre-launch "超前邀约内测" (invited early-access beta), Kling partner. The description credits multiple keyframes and 30s generation for the dialogue between two geese and a desert music video. That is a creator claim. Output only.
- **New: Eren Şerefoğlu,** https://www.youtube.com/watch?v=yNvj7a1u8No (2026-10-16 08:20 Taipei, 12s). Contest entry, unconfirmed.

### 4.4 Flash-only (excluded)
The v1 list of 20 plus c5vn2D74wOU, SbRna_uB9aI and TMdgRPQCJc4.

### 4.5 X (labelled separately; times are Taipei)
- **X1 EndFolding79421,** https://x.com/EndFolding79421/status/2110800090897973405 (10-16 02:28). 30.04s, full story prompt disclosed. Unchanged.
- **X2 marco_a_b_c,** https://x.com/marco_a_b_c/status/2110830419641811123 (10-16 04:29). 30.02s, "four keyframes", watermark. Unchanged.
- **X3 AIWarper,** https://x.com/AIWarper/status/2110833050955526292 (10-16 04:39). 10.0s, "10 keyframes". Unchanged.
- **X4 TechHalla:** see M4.
- **X5 (NEW) Dheepanratnam:** result https://x.com/Dheepanratnam/status/2110757536102055949, prompt in the same post, 10-15 23:39 (39 minutes after launch).
  - 30.04s at 1080x1920, which confirms it is not Flash.
  - The prompt is a timed beat sheet for a London street interview (0:00–0:30) with an elderly woman and a cat.
  - **Beat check from 1s frames plus transcript:**
    - Dialogue lines arrive roughly in order. "Three things, darling" starts at about 0:03, versus 0:07 in the prompt. "The cat's my lawyer" at about 0:20 is inside its 0:17–0:22 window.
    - The 0:03–0:07 "lowers her glasses" beat was not seen; her glasses stay on in the sampled frames.
    - The cat switching off the mic (0:22–0:27) was not seen in the sampled frames.
    - She walks off from about 0:25 (prompt says 0:27), and the shot changes to a wide.
    - Woman and cat look consistent throughout the sampled frames.
  - The first post in the thread (https://x.com/Dheepanratnam/status/2110757532457386393) is a 51s overview of Kling's features, not the test.
- **X6 (NEW) Dani__oros,** https://x.com/Dani__oros/status/2110790297458544971 (10-16 01:49). "My first fight test… came out better than I thought it would, considering how vague my prompt was." Anime fight, 30.09s. Prompt not disclosed.
- **X7 (NEW) HeyZoyaKhan,** https://x.com/HeyZoyaKhan/status/2110755315834827162 (10-15 23:30, 30 minutes after launch, 31.8K impressions).
  - Tarzan rides a wolf with a forest army, 30.19s, "KlingAI 4.0" watermark visible.
  - Workflow reply: "Omni Reference… Native 30-second generation… 1080p" (https://x.com/HeyZoyaKhan/status/2110755356276412552). The prompt itself was not found in the thread.
  - In sampled frames around 0:17–0:20, the rider and mount look different from the opening shots. Whether that is intended is unknown.
  - The post was this early and had this much reach, so treat it as likely early-access or partner content (unknown).
- **X8 (NEW) Starjupi,** https://x.com/Starjupi/status/2110781205415104571 (10-16 01:13). Turtle plumber "Frank", 30.09s, tagged #klingECP (Kling's creator program). The workflow "in the comments" was not read.
- **Unconfirmed:** SilentNightX97 2110786321459622080 (15s, DeepSeek-written prompt); shishirdotai 2110776884774773204 (9s).
- **Comments:**
  - SaindoMatrix, https://x.com/SaindoMatrix/status/2110827040828195097: Kling 4 "nailed it in the first try" after a week of failing with Kling 3.
  - bLot7d, https://x.com/bLot7d/status/2110894994303373338: the real bar is a "3-shot dialogue scene where eyelines and character consistency survive across cuts."
  - TechHalla reply: "I had to change the prompting I was used to use a bit" (https://x.com/techhalla/status/2110819496911122803).
- **Reddit:** only the v1 snippet (u/Alyssa_Koch, sponsored, thread unopened).

## 5. (B) Candidate excerpts (18). Permission for all: needed, none granted, none requested.

| # | Source | Timestamp | Shows | Q | Credit |
|---|---|---|---|---|---|
| E1 | M1 Oprelia | 19:09–20:32 | Keyframe UI; bird test with broken start and missing middle frame | Q3 | Oprelia AI, YouTube |
| E2 | M1 | 16:00–16:42 | Non-keyframed rooftop fight breaking apart; position jumps | Q2 | Oprelia AI |
| E3 | M1 | 18:20–19:08 | Retry still distorted; "another one that I deleted" | Q4 | Oprelia AI |
| E4 | M1 | 14:30–14:49 | 14s Pixar clip; line cut off | Q1/Q4 | Oprelia AI |
| E5 | M1 | 17:03–17:52 | Realism dialogue + voice reference | Q5 | Oprelia AI |
| E6 | M2 Starky | ~4:00 | "VIDEO 4.0 Preview · 1080p · 30s" panel | Spec | Matt Starky, YouTube |
| E7 | M2 | 0:51–1:05 | "Full UGC ad in one generation" claim | Q4 | Matt Starky |
| E8 | M2 | ~4:14–4:40 | 30s UGC output | Q1/Q5 | Matt Starky |
| E9 | M3 AiHustleGame | 4:05–5:20 | 10s shots, regenerate, trim in Premiere | Q4 | AiHustleGame (Kling partner) |
| E10 | X1 EndFolding79421 | 0:00–0:30 | 30s single story prompt | Q1 | @EndFolding79421, X |
| E11 | X2 / X3 | 0:00–0:30 / 0:00–0:10 | 4 keyframes in 30s; 10 keyframes in 10s | Q3 | @marco_a_b_c / @AIWarper, X |
| E12 | M4 TechHalla | 2:52–3:00 + prompt card 01 (X image) | 5 hard cuts in a 7s generation | Q2 | TechHalla, YouTube/X |
| E13 | M4 | 5:40–5:48 + card 03 | 6 refs, 4 heroes, 8s, on-model | Q1 | TechHalla |
| E14 | M4 | 6:09–6:15 + card 02 | One prompt, three camera setups, 8s | Q2 | TechHalla |
| E15 | M1 Oprelia | 20:36–21:34 | Keyframed alien-boxing fight, "best video out of the bunch" | Q2/Q3 | Oprelia AI |
| E16 | M5 Donis | 4:27–4:51 | Kling 24s 5-shot interrogation; reverse angles | Q1 | The AI Filmmaking Advantage (Paul Donis), YouTube (Kling partner) |
| E17 | M5 Donis | 1:34–2:28 | 27s Blender-guided robot-army test, Kling vs Seedance, same input | Q2/Q4 | Same |
| E18 | X5 Dheepanratnam | 0:00–0:30 + prompt | Timed beat sheet vs result | Q3 | @Dheepanratnam, X |
| E19 | M6 kzhu | 0:10–1:10 | Pelican benchmark failures | Q2/Q5 | AI产品狙击手 kzhu, YouTube |
| E20 | C4 Kling × Simon Meyer (**official**) | 2:12–2:58 | "50 times on this one shot"; ~80% lip sync | Q4 | Kling AI official |

The table has 20 rows. Pick 16–18; E11 and E20 are the most optional.

## 6. (C) Attributable comments

The list now has 6.
- **SaindoMatrix** (above).
- **AiHustleGame:** "A 10 second generation does not mean I need all 10 seconds" (4:38).
- **Simon Meyer** (official video, 2:14).
- **bLot7d** (above).
- **Paul Donis**, thread opener (above).
- **Dani__oros:** "better than I thought it would, considering how vague my prompt was" (above).

## 7. Findings on the five questions (no controlled comparisons)

1. **Consistency.**
   - Sampled frames suggest identity holds in single 30s generations: EndFolding, Dheepanratnam, Starky.
   - Donis's 24s, 5-shot Kling interrogation keeps two characters consistent in sampled frames. Eyelines were not assessed.
   - TechHalla's 6-reference consistency was shown in **8s** clips.
   - Counter-signals: HeyZoyaKhan's mid-clip rider/mount change (intent unknown), marco's possible drift at about 0:05, and Oprelia's position jumps.
2. **Motion.**
   - Fast fights without keyframes break apart (Oprelia 16:18, 18:20–18:49).
   - Oprelia's keyframed fight was the best result of the session (20:42–20:52).
   - TechHalla claims 5 clean cuts in 7s.
   - kzhu's pelican benchmark shows object and physics errors.
3. **Keyframes and timed beats.**
   - The control is real but approximate. Oprelia calls keyframes the most control available, but the bird test's start broke and a middle frame went missing.
   - Dheepanratnam's timed prompt landed its dialogue roughly on time but skipped two action beats in sampled frames.
4. **Work saved vs retakes.**
   - The "30s replaces stitching" claim comes from Starky and from Kling.
   - Practice so far is shorter than 30s. Oprelia's tests ran 10–20s; TechHalla's showcased clips ran 7–8s; AiHustleGame used 10s shots and trimmed; Donis's longest were 24–27s.
   - Retakes: Oprelia deleted attempts; Simon Meyer did 50 on one shot (official video). Donis showed first takes only, but didn't say how many prompts or setups he discarded beforehand (unknown).
5. **Usable footage.**
   - Strongest: realistic dialogue, lip sync and voice reference (Oprelia, Simon Meyer); single-presenter UGC and street interviews (Starky, Dheepanratnam); reference-locked short multi-cut action (TechHalla).
   - Weakest: fast choreography without keyframes, anime backgrounds, physics-heavy object scenes (kzhu).

## 8. (E) Fact-check list

1. Launch time, 15:00 UTC Oct 15. Confirmed.
2. Flash limits. Confirmed (feature page).
3. 4K availability. Not verified.
4. API date. Not verified; Oprelia says Oct 21, Kling says "coming soon".
5. "840" on Starky's Generate button. The unit is not labelled.
6. Starky's "VIDEO 4.0 Preview" label. Seen at 360p; recheck at higher resolution.
7. AiHustleGame full vs Flash. Unconfirmed.
8. TechHalla's 7–8s and 1080p. Confirmed from his own cards. "One generation" is his claim.
9. E14 timestamps. Located in the X copy; the YouTube times are inferred from matching duration and chapters, so recheck on YouTube.
10. Oprelia quotes. Re-checked with a larger transcription model; listen once more before recording.
11. Donis's method claims ("first takes only, same inputs"). These are his claims. The resolution differences and Topaz upscale are disclosed.
12. Dheepanratnam beat check. Based on 1s frame sampling. A missed beat could fall between samples, so re-watch before stating.
13. kzhu's failures. From his voice-over and description, not checked against the video ourselves.
14. HeyZoyaKhan rider/mount change. Seen in 2.5s samples; re-watch.
15. Kling ToS 4.6 does not grant us rights. Confirmed.
16. Reddit snippet. Thread not opened.

## 9. (F) Evidence-led sequence for ~10 minutes

Each block is either an evidence block or a labelled non-test block.
1. Cold open with the official claim (non-test, 0:30).
2. Flash vs full, why it matters, how tests were sorted (non-test spec, 1:00).
3. 30s single takes: EndFolding, Dheepanratnam, Starky (1:15).
4. The stitching claim, then what creators actually generated: TechHalla's 7–8s cards, AiHustleGame's 10s, Oprelia's 10–20s (1:15).
5. Keyframes: Oprelia bird test vs keyframed fight; marco and AIWarper; Dheepanratnam's beat sheet (1:30).
6. Where it breaks: Oprelia's non-keyframed fights; kzhu's pelican benchmark; clipped line (1:15).
7. Same-prompt first takes: Donis's robot army and interrogation, with caveats (1:00).
8. Retakes and cost: Oprelia's deletions, Simon Meyer (official), 840 unverified, credit rates unpublished (0:45).
9. Decision framework (non-test, 1:00).
10. Close: bLot7d's test, and Donis's 24s scene as a partial answer (0:30).

That totals about 10:00. Test evidence fills about 7:00; labelled non-test material fills about 3:00.

## 10. Gaps
- Still no retake counts per 30s generation.
- No published credit rates.
- Donis's prompts are too small to read at 360p.
- Starjupi's workflow comments and HeyZoyaKhan's prompt were not found.
- Chinese platforms were inaccessible, so Chinese coverage rests only on kzhu and AIFC.
- No end-to-end viewing.

## 11. Changes from v1
- **Added:** M5, M6, X5–X8, AIFC, Eren, and 3 Flash exclusions.
- **TechHalla corrected:** 7–8s clips, confirmed via 1080p cards, E14 located.
- **Oprelia:** prompts transcribed; quotes re-timed (the 20:25 quote is now 20:32); keyframed fight added as the creator's best result.
- **Q2 and Q4 findings revised.**
- **Runtime:** 4.5–5 min → about 10 min with labelled non-test segments.

## 12. Official stills (PDF only)
Three images from Kling's blog: title card, keyframe timeline UI, canvas UI. © Kling AI/Kuaishou, for internal reference only. Video use needs Kling's permission.
