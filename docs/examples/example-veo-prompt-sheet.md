# Veo Prompt Sheet

## 1. Scene Identity
- Project: Borrowed Light
- Scene ID: SC-04
- Scene Title: Laundromat Promise
- Version: v1

## 2. Scene Summary
- What the scene needs to communicate: A damaged relationship shifts because proof is returned before forgiveness is spoken.
- Emotional destination: Tentative trust without full reconciliation.

## 3. Global Continuity Anchors
- Character anchors: Sana in a navy diner uniform with folded sleeves and tired eyes; Ray in a wet red hoodie with a messenger bag
- Environment anchors: Small fluorescent laundromat, rain-streaked front windows, rotating washers, metal folding counter
- Prop anchors: Dented cassette case with a worn handwritten label
- Camera-language anchors: Controlled, intimate, realistic, subtle motion only
- Color / lighting anchors: Cool fluorescent overheads, soft neon reflections, warm skin tones against a colder room
- Audio anchors: Washer hum, rain hiss, occasional bell or contact sounds, naturalistic dialogue

## 4. Global Prompting Rules
- Keep the scene grounded and emotionally restrained
- Reuse the same character and environment wording across all prompts
- Preserve rain visibility and cassette continuity
- Let silence and room tone matter as much as dialogue

## 5. Shot Execution Plan

### Shot S1 - Sana Alone At The Counter
- Execution mode: `single-prompt shot`
- Why this mode was chosen: One visual beat with stable camera movement fits comfortably in one generation
- Required references: Sana character reference, laundromat environment reference
- Continuity anchors for this shot: Rain visible behind Sana, folded uniforms on the counter, washers moving in the background

#### Prompt / Segment S1-A
- Purpose: Establish Sana's tired routine before Ray enters
- Base Veo prompt: Slow intimate push-in through a late-night laundromat toward Sana, a tired young woman in a navy diner uniform with folded sleeves, quietly folding work clothes at a metal counter, rotating washers glowing behind her, rain streaking the front windows, grounded contemporary realism, cool fluorescent light with soft neon reflections, restrained camera movement, subtle cinematic texture.
- Audio guidance: Constant washer hum, soft rain on glass, no dialogue, no dramatic score swell.
- Negative constraints: No extra customers, no glamorized fashion styling, no exaggerated camera shake, no sudden smile.
- Stitch or timing notes: None.
- Retry variants: Tighter push-in on Sana's hands first, or a slightly wider opening that keeps more washer movement in frame.

### Shot S2 - Ray Enters And Reveals The Tape
- Execution mode: `stitched multi-prompt shot`
- Why this mode was chosen: The editorial intent is one uninterrupted entrance shot, but the action and line delivery exceed a safe single Veo clip.
- Required references: Ray character reference, laundromat environment reference, cassette prop reference, bridge-frame pair
- Continuity anchors for this shot: Red hoodie remains visibly wet, messenger bag stays on Ray's shoulder until he nears the counter, cassette appears in his raised hand after he enters

#### Prompt / Segment S2-A
- Purpose: Capture the bell, doorway interruption, and Ray's entrance
- Base Veo prompt: Continuous handheld-but-controlled realist shot from inside a small fluorescent laundromat as the front door opens, a bell rings, and Ray enters from the rainy night wearing a wet faded red hoodie and messenger bag, pausing just inside the doorway before lifting a dented cassette case into view, intimate urban drama, cool fluorescent light, rain glowing in the glass, grounded performance focus.
- Audio guidance: Bell cue at entry, rain briefly louder as the door opens, wet footsteps beginning, Ray says clearly, "I found it."
- Negative constraints: No dramatic sprinting, no extra props in his hands, no romantic smile, no stylized slow motion.
- Stitch or timing notes: End with Ray mid-crossing toward the counter, body angled three-quarters toward Sana, cassette still visible in hand.
- Retry variants: Shorter doorway pause, or a cleaner reveal of the cassette before he steps forward.

#### Prompt / Segment S2-B
- Purpose: Continue the same shot seamlessly as Ray crosses the room toward Sana
- Base Veo prompt: Seamless continuation of the same late-night laundromat entrance shot, matching Ray's wet red hoodie, messenger bag, posture, and cassette position as he crosses from the doorway toward the metal folding counter where Sana stands off-frame, controlled tracking motion, persistent washer glow, rain still streaking the windows, grounded emotional realism, no visible edit.
- Audio guidance: Continue washer hum and soft wet footsteps under the room tone after the line lands.
- Negative constraints: No change in wardrobe dryness, no teleporting bag or cassette, no new extras, no shift to a different room layout.
- Stitch or timing notes: Match the end pose of S2-A; hide the seam inside motion and footstep continuity.
- Retry variants: Slightly faster crossing pace, or a wider track that keeps both doorway and counter relationship clear.

### Shot S3 - Sana Holds The Silence
- Execution mode: `single-prompt shot`
- Why this mode was chosen: One reaction beat with controlled stillness works best as a short isolated generation
- Required references: Sana character reference, laundromat environment reference
- Continuity anchors for this shot: Sana remains guarded, rain and washers stay present but soft, eyeline matches Ray's position at the counter

#### Prompt / Segment S3-A
- Purpose: Let Sana's silence carry judgment
- Base Veo prompt: Tight realistic over-the-shoulder shot from Ray's side onto Sana at the folding counter in the fluorescent laundromat, Sana in a navy diner uniform holding still after hearing "I found it," her expression guarded and exhausted, rotating washer lights and rain-blurred windows soft behind her, minimal camera drift, intimate emotional realism.
- Audio guidance: No dialogue, just washer hum, rain, and a brief feeling of held breath in the room.
- Negative constraints: No immediate smile, no melodramatic tears, no camera whip.
- Stitch or timing notes: None.
- Retry variants: Slightly tighter framing on Sana's eyes, or a version with less camera drift.

### Shot S4 - Cassette On The Counter
- Execution mode: `single-prompt shot`
- Why this mode was chosen: One tactile action beat with one spoken line fits cleanly in one generation
- Required references: Ray character reference, cassette prop reference, counter detail
- Continuity anchors for this shot: Cassette dent remains visible, counter surface consistent, Ray's sleeve still damp

#### Prompt / Segment S4-A
- Purpose: Make the apology physical through the tape placement
- Base Veo prompt: Medium close realistic shot focused on Ray's hand setting a dented cassette case onto a metal folding counter in a small late-night laundromat, Sana just at the edge of frame, Ray's damp red hoodie sleeve visible, subtle lateral camera follow, grounded urban drama, cool fluorescent light and soft reflections, tactile emphasis on the object landing.
- Audio guidance: Crisp cassette contact on metal, Ray quietly says, "I should've come back sooner."
- Negative constraints: No aggressive slam, no extreme close-up abstraction, no sudden style change.
- Stitch or timing notes: None.
- Retry variants: Stronger focus on the cassette label, or slightly slower hand movement to make the landing feel deliberate.

### Shot S5 - Then Stay
- Execution mode: `timestamped multi-beat sequence`
- Why this mode was chosen: The shot needs a held shared frame with a timed handoff, look, and final line inside one emotionally coherent beat
- Required references: Sana character reference, Ray character reference, cassette prop reference, optional two-shot composition frame
- Continuity anchors for this shot: Cassette moves from counter to Sana's hand, Ray stays still and vulnerable, rain remains visible in the background

#### Prompt / Segment S5-A
- Purpose: Carry the final handoff and line in one shared frame
- Base Veo prompt: Intimate realistic two-shot in a fluorescent late-night laundromat, Sana in a navy diner uniform lifts the dented cassette from the metal counter, looks at Ray in his wet red hoodie, and after a measured beat quietly says, "Then stay," with restrained camera drift, rain-streaked windows and washer glow behind them, contemporary grounded drama, cool fluorescent palette with warm skin tones.
- Audio guidance: 0:00-0:03 washer hum and rain only as Sana takes the cassette, 0:03-0:06 small room-breath pause, 0:06-0:08 Sana says clearly, "Then stay."
- Negative constraints: No kiss, no embrace, no triumphant music, no sudden bright lighting shift.
- Stitch or timing notes: Preserve shared framing and leave a soft breath after the line.
- Retry variants: A version with slightly more space between them, or a version with a slower look-up before the final line.

## 6. Scene-Level Risks
- Most likely continuity failures: Ray drying out between shots, cassette dent disappearing, laundromat palette shifting warmer, emotion becoming too romantic too early
- First things to retry if outputs drift: Reassert character wardrobe anchors, cassette damage, and the "grounded restrained realism" language before changing anything else
