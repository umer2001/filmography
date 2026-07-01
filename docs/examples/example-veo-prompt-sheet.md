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
- Prompt style family: `cinematic-atmospheric`
- Why this prompt style was chosen: The shot's job is to establish isolation, environment, and mood before dialogue begins.
- Required references: Sana character reference, laundromat environment reference
- Continuity anchors for this shot: Rain visible behind Sana, folded uniforms on the counter, washers moving in the background

#### Prompt / Segment S1-A
- Purpose: Establish Sana's tired routine before Ray enters
- Formula coverage:
  - Shot composition: Slow intimate push-in through the laundromat toward the folding counter
  - Subject details: Sana in navy diner uniform with folded sleeves and tired eyes
  - Action: Quietly folding work clothes without looking up
  - Setting / environment: Late-night laundromat, rotating washers, rain-streaked windows
  - Aesthetics / mood: Grounded realism, cool fluorescent light, restrained melancholy
  - Audio: Washer hum and soft rain, no dialogue
- Base Veo prompt: Slow intimate push-in through a late-night laundromat toward Sana, a tired young woman in a navy diner uniform with folded sleeves, quietly folding work clothes at a metal counter, rotating washers glowing behind her, rain streaking the front windows, grounded contemporary realism, cool fluorescent light with soft neon reflections, restrained camera movement, subtle cinematic texture.
- Audio guidance: Constant washer hum, soft rain on glass, no dialogue, no dramatic score swell.
- Negative constraints: No extra customers, no glamorized fashion styling, no exaggerated camera shake, no sudden smile.
- Stitch or timing notes: None.
- Retry variants: Tighter push-in on Sana's hands first, or a slightly wider opening that keeps more washer movement in frame.

### Shot S2 - Ray Enters And Reveals The Tape
- Execution mode: `stitched multi-prompt shot`
- Why this mode was chosen: The editorial intent is one uninterrupted entrance shot, but the action and line delivery exceed a safe single Veo clip.
- Prompt style family: `character-dialogue` with `cinematic-atmospheric` secondary
- Why this prompt style was chosen: The line "I found it" and Ray's hesitant performance are the point, while the rain-soaked room must remain atmospheric.
- Required references: Ray character reference, laundromat environment reference, cassette prop reference, bridge-frame pair
- Continuity anchors for this shot: Red hoodie remains visibly wet, messenger bag stays on Ray's shoulder until he nears the counter, cassette appears in his raised hand after he enters

#### Prompt / Segment S2-A
- Purpose: Capture the bell, doorway interruption, and Ray's entrance
- Formula coverage:
  - Shot composition: Continuous controlled shot from inside the laundromat toward the door
  - Subject details: Ray in wet faded red hoodie with messenger bag and dented cassette case
  - Action: Door opens, Ray pauses, lifts the cassette, and speaks
  - Setting / environment: Small fluorescent laundromat, rainy night outside, glass glowing with rain
  - Aesthetics / mood: Grounded performance focus, intimate urban drama
  - Audio: Bell cue, rain swell, wet footsteps, locked dialogue, no subtitles
- Base Veo prompt: Continuous handheld-but-controlled realist shot from inside a small fluorescent laundromat as the front door opens, a bell rings, and Ray enters from the rainy night wearing a wet faded red hoodie and messenger bag, pausing just inside the doorway before lifting a dented cassette case into view, intimate urban drama, cool fluorescent light, rain glowing in the glass, grounded performance focus.
- Audio guidance: Bell cue at entry, rain briefly louder as the door opens, wet footsteps beginning, Ray says clearly, "I found it." No subtitles.
- Negative constraints: No dramatic sprinting, no extra props in his hands, no romantic smile, no stylized slow motion.
- Stitch or timing notes: End with Ray mid-crossing toward the counter, body angled three-quarters toward Sana, cassette still visible in hand.
- Retry variants: Shorter doorway pause, or a cleaner reveal of the cassette before he steps forward.

#### Prompt / Segment S2-B
- Purpose: Continue the same shot seamlessly as Ray crosses the room toward Sana
- Formula coverage:
  - Shot composition: Seamless tracking continuation from doorway toward counter
  - Subject details: Ray's wet red hoodie, messenger bag, posture, and cassette position match S2-A
  - Action: Ray crosses toward Sana without losing the cassette reveal
  - Setting / environment: Same laundromat layout, washer glow, rain-streaked windows
  - Aesthetics / mood: Controlled realism, no visible edit, restrained tension
  - Audio: Washer hum and wet footsteps continue under room tone
- Base Veo prompt: Seamless continuation of the same late-night laundromat entrance shot, matching Ray's wet red hoodie, messenger bag, posture, and cassette position as he crosses from the doorway toward the metal folding counter where Sana stands off-frame, controlled tracking motion, persistent washer glow, rain still streaking the windows, grounded emotional realism, no visible edit.
- Audio guidance: Continue washer hum and soft wet footsteps under the room tone after the line lands.
- Negative constraints: No change in wardrobe dryness, no teleporting bag or cassette, no new extras, no shift to a different room layout.
- Stitch or timing notes: Match the end pose of S2-A; hide the seam inside motion and footstep continuity.
- Retry variants: Slightly faster crossing pace, or a wider track that keeps both doorway and counter relationship clear.

### Shot S3 - Sana Holds The Silence
- Execution mode: `single-prompt shot`
- Why this mode was chosen: One reaction beat with controlled stillness works best as a short isolated generation
- Prompt style family: `character-dialogue`
- Why this prompt style was chosen: This is a performance beat where silence and eyeline carry the emotional power.
- Required references: Sana character reference, laundromat environment reference
- Continuity anchors for this shot: Sana remains guarded, rain and washers stay present but soft, eyeline matches Ray's position at the counter

#### Prompt / Segment S3-A
- Purpose: Let Sana's silence carry judgment
- Formula coverage:
  - Shot composition: Tight over-the-shoulder shot from Ray's side onto Sana
  - Subject details: Sana in navy diner uniform, guarded and exhausted
  - Action: Sana holds still and refuses to answer
  - Setting / environment: Folding counter, fluorescent laundromat, soft washer lights and rain windows
  - Aesthetics / mood: Minimal drift, intimate emotional realism
  - Audio: No dialogue, washer hum, rain, held room tone
- Base Veo prompt: Tight realistic over-the-shoulder shot from Ray's side onto Sana at the folding counter in the fluorescent laundromat, Sana in a navy diner uniform holding still after hearing "I found it," her expression guarded and exhausted, rotating washer lights and rain-blurred windows soft behind her, minimal camera drift, intimate emotional realism.
- Audio guidance: No dialogue, just washer hum, rain, and a brief feeling of held breath in the room.
- Negative constraints: No immediate smile, no melodramatic tears, no camera whip.
- Stitch or timing notes: None.
- Retry variants: Slightly tighter framing on Sana's eyes, or a version with less camera drift.

### Shot S4 - Cassette On The Counter
- Execution mode: `single-prompt shot`
- Why this mode was chosen: One tactile action beat with one spoken line fits cleanly in one generation
- Prompt style family: `product-showcase` with `character-dialogue` secondary
- Why this prompt style was chosen: The cassette is the story proof, so the object detail and contact sound need product-level clarity while the apology remains naturalistic.
- Required references: Ray character reference, cassette prop reference, counter detail
- Continuity anchors for this shot: Cassette dent remains visible, counter surface consistent, Ray's sleeve still damp

#### Prompt / Segment S4-A
- Purpose: Make the apology physical through the tape placement
- Formula coverage:
  - Shot composition: Medium close shot on Ray's hand and the metal counter
  - Subject details: Dented cassette case, damp red hoodie sleeve, Sana at frame edge
  - Action: Ray sets the cassette down and quietly apologizes
  - Setting / environment: Small late-night laundromat counter under fluorescent light
  - Aesthetics / mood: Tactile grounded drama, soft reflections, deliberate movement
  - Audio: Crisp cassette contact, apology line, no subtitles
- Base Veo prompt: Medium close realistic shot focused on Ray's hand setting a dented cassette case onto a metal folding counter in a small late-night laundromat, Sana just at the edge of frame, Ray's damp red hoodie sleeve visible, subtle lateral camera follow, grounded urban drama, cool fluorescent light and soft reflections, tactile emphasis on the object landing.
- Audio guidance: Crisp cassette contact on metal, Ray quietly says, "I should've come back sooner." No subtitles.
- Negative constraints: No aggressive slam, no extreme close-up abstraction, no sudden style change.
- Stitch or timing notes: None.
- Retry variants: Stronger focus on the cassette label, or slightly slower hand movement to make the landing feel deliberate.

### Shot S5 - Then Stay
- Execution mode: `timestamped multi-beat sequence`
- Why this mode was chosen: The shot needs a held shared frame with a timed handoff, look, and final line inside one emotionally coherent beat
- Prompt style family: `character-dialogue` with `cinematic-atmospheric` secondary
- Why this prompt style was chosen: The final line and timed pause carry the emotional release, while the room tone keeps the scene restrained.
- Required references: Sana character reference, Ray character reference, cassette prop reference, optional two-shot composition frame
- Continuity anchors for this shot: Cassette moves from counter to Sana's hand, Ray stays still and vulnerable, rain remains visible in the background

#### Prompt / Segment S5-A
- Purpose: Carry the final handoff and line in one shared frame
- Formula coverage:
  - Shot composition: Intimate realistic two-shot with restrained drift
  - Subject details: Sana in navy diner uniform, Ray in wet red hoodie, dented cassette
  - Action: Sana takes cassette, looks at Ray, waits, then speaks
  - Setting / environment: Fluorescent late-night laundromat with rain windows and washer glow
  - Aesthetics / mood: Fragile restrained realism, cool palette with warm skin tones
  - Audio: Timed room tone, final locked line, no subtitles
- Base Veo prompt: Intimate realistic two-shot in a fluorescent late-night laundromat, Sana in a navy diner uniform lifts the dented cassette from the metal counter, looks at Ray in his wet red hoodie, and after a measured beat quietly says, "Then stay," with restrained camera drift, rain-streaked windows and washer glow behind them, contemporary grounded drama, cool fluorescent palette with warm skin tones.
- Audio guidance: 0:00-0:03 washer hum and rain only as Sana takes the cassette, 0:03-0:06 small room-breath pause, 0:06-0:08 Sana says clearly, "Then stay." No subtitles.
- Negative constraints: No kiss, no embrace, no triumphant music, no sudden bright lighting shift.
- Stitch or timing notes: Preserve shared framing and leave a soft breath after the line.
- Retry variants: A version with slightly more space between them, or a version with a slower look-up before the final line.

## 6. Scene-Level Risks
- Most likely continuity failures: Ray drying out between shots, cassette dent disappearing, laundromat palette shifting warmer, emotion becoming too romantic too early
- First things to retry if outputs drift: Reassert character wardrobe anchors, cassette damage, and the "grounded restrained realism" language before changing anything else

## 7. Sample Prompt Library From Veo 3.1 Guide

Use these as style references when selecting prompt families for new shots. They are not part of the Borrowed Light scene; they show how different use cases shape camera, subject, action, setting, aesthetics, and audio.

### Sample 1 - Melancholic Bus Window
- Prompt style family: `cinematic-atmospheric`
- Use case: Emotional storytelling, music videos, narrative films
- Sample prompt: `Close-up with very shallow depth of field, a young woman's face, looking out a bus window at the passing city lights with her reflection faintly visible on the glass, inside a bus at night during a rainstorm, melancholic mood with cool blue tones, moody, cinematic.`

### Sample 2 - Frost-Covered Bridge
- Prompt style family: `cinematic-atmospheric`
- Use case: Contemplative scenes, establishing shots, atmospheric content
- Sample prompt: `A wide, eye-level cinematic shot captures a man walking slowly across a frost-covered bridge at dawn, his hands tucked into the pockets of a heavy coat. Pale morning light glows faintly through soft, curling fog that clings to the bridge railings. In the distance, bare trees fade into the mist, their skeletal branches barely visible. The pace is unhurried and reflective, evoking a naturalistic and quiet mood.`

### Sample 3 - Emotional Window Moment
- Prompt style family: `character-dialogue` with `cinematic-atmospheric` secondary
- Use case: Dramatic moments, character development, transitions
- Sample prompt: `Intimate close-up of a young adult at a rain-streaked window, soft backlight shaping silhouette. Slow push-in. Gentle piano and rain ambience. He whispers, "I'm ready." No subtitles.`

### Sample 4 - Historical Cartographer
- Prompt style family: `character-dialogue`
- Use case: Adventure narratives, historical content, exposition scenes
- Sample prompt: `A medium shot, historical adventure setting: Warm lamplight illuminates a cartographer in a cluttered study, poring over an ancient, sprawling map spread across a large table. Cartographer: "According to this old sea chart, the lost island isn't myth! We must prepare an expedition immediately!"`

### Sample 5 - Old Sailor Character
- Prompt style family: `character-dialogue`
- Use case: Character introductions, maritime content, poetic dialogue
- Sample prompt: `A medium shot frames an old sailor, his knitted blue sailor hat casting a shadow over his eyes, a thick grey beard obscuring his chin. He holds his pipe in one hand, gesturing with it towards the churning, grey sea beyond the ship's railing. "This ocean, it's a force, a wild, untamed might. And she commands your awe, with every breaking light."`

### Sample 6 - Business Professional Working
- Prompt style family: `professional-business`
- Use case: Corporate videos, stock footage, training materials
- Sample prompt: `30-year-old woman in business casual attire typing on laptop at modern wooden desk, side angle medium shot, natural window lighting from left, focused expression, contemporary office with plants visible in background.`

### Sample 7 - Thermal Home Cross-Section
- Prompt style family: `professional-business`
- Use case: Educational content, explainer videos, technical documentation
- Sample prompt: `Cross-section view of home showing how heat escapes through windows and walls, thermal imaging effect with color-coded temperature zones, animated arrows indicating heat loss patterns, slow methodical camera movement explaining each area, educational documentary style.`

### Sample 8 - Product On Rotating Pedestal
- Prompt style family: `product-showcase`
- Use case: E-commerce, product launches, advertising
- Sample prompt: `A luxury smartwatch sits on a rotating pedestal inside a dark studio. Studio lights highlight its polished metal surface and intricate details. The camera orbits smoothly 360 degrees around the product. Soft mechanical sounds play as the pedestal rotates. Modern, minimal aesthetic with shallow depth of field.`

### Sample 9 - Product Montage
- Prompt style family: `product-showcase`
- Use case: Tech demos, app showcases, quick product highlights
- Sample prompt: `Fast three-beat montage: 1) close-up button press; 2) medium shot product in use; 3) wide shot satisfied user. Crisp snap sound for each beat, then a short swell. High-key lighting, modern color grade. She says, "Done." No subtitles.`

### Sample 10 - Product Assembly Animation
- Prompt style family: `product-showcase` with `professional-business` secondary
- Use case: Assembly instructions, how-to videos, user guides
- Sample prompt: `An animated step-by-step demonstration shows product assembly with clear labeled arrows and instructional text. Clean white background keeps focus on the assembly steps. Camera slowly zooms in on each highlighted step. Professional voice explains: "First, align the main components carefully." Soft corporate music underneath. Each step completes with satisfying click sound.`

### Sample 11 - Chef Preparing Food
- Prompt style family: `culinary-food`
- Use case: Cooking tutorials, restaurant marketing, food content
- Sample prompt: `Confident chef in white uniform chopping fresh vegetables on bamboo cutting board. Close-up side angle captures precise knife technique. Natural kitchen lighting from window creates soft shadows. Sounds of knife on cutting board with gentle kitchen ambiance. Professional culinary aesthetic.`

### Sample 12 - Coffee Shop Latte Art
- Prompt style family: `culinary-food`
- Use case: Cafe marketing, coffee tutorials, lifestyle content
- Sample prompt: `Medium close-up of a barista pouring steamed milk into a ceramic coffee cup, creating intricate latte art. Morning sunlight streams through large windows behind, illuminating rising steam. Camera captures the pour in slow motion from a side angle. Sounds include the gentle hiss of the steam wand, soft cafe chatter, and acoustic guitar music. Warm and inviting atmosphere.`

### Sample 13 - City Skyline Time-Lapse
- Prompt style family: `landscape-environment` with `transformation-timelapse` secondary
- Use case: City documentaries, time-lapse sequences, establishing shots
- Sample prompt: `A time-lapse of a bustling city skyline as day transitions to night. The camera is static. Watch as the sun sets, casting long shadows, and the city lights begin to twinkle on, with streaks of car headlights moving along the streets below.`

### Sample 14 - Tropical Island Aerial
- Prompt style family: `landscape-environment`
- Use case: Travel videos, resort marketing, vacation content
- Sample prompt: `A drone camera starts at beach level on white sand and steadily rises to reveal an entire tropical island from above. The ocean water transitions from crystal clear turquoise near the shore to deep blue farther out. Golden hour sunlight bathes the scene in warm tones. Gentle wave sounds blend with distant seabird calls. Relaxed tropical music.`

### Sample 15 - Thunderstorm Approaching
- Prompt style family: `landscape-environment` with `cinematic-atmospheric` secondary
- Use case: Nature documentaries, dramatic b-roll, weather content
- Sample prompt: `Wide shot of dark storm clouds rolling dramatically across the sky over an open wheat field. Strong wind bends the grain in visible waves. Camera starts wide and slowly pushes forward toward the storm front. Lightning flashes illuminate clouds from within. Thunder rumbles with increasing intensity as wind builds. Powerful orchestral music enhances the raw power of nature.`

### Sample 16 - Vintage 1920s Street
- Prompt style family: `stylized-creative`
- Use case: Period pieces, historical content, retro aesthetics
- Sample prompt: `A vintage 1920s street scene, sepia toned, film grain, with characters in period attire walking along cobblestone streets. Vintage cars pass by. Jazz music plays faintly from a nearby club. Atmospheric and nostalgic mood.`

### Sample 17 - Anime Style Character
- Prompt style family: `stylized-creative`
- Use case: Animated content, fantasy storytelling, manga-inspired videos
- Sample prompt: `A dynamic scene in a vibrant Japanese anime style. A magical girl with silver hair and glowing blue eyes walks in a forest. The style features sharp lines, bright, saturated colors, and expressive character design.`

### Sample 18 - Forgotten City Scene
- Prompt style family: `sci-fi-fantasy` with `cinematic-atmospheric` secondary
- Use case: Post-apocalyptic content, sci-fi narratives, concept videos
- Sample prompt: `The scene is a rain-slicked, crumbling street in a forgotten city, shrouded in perpetual twilight. Giant, bioluminescent mushrooms have sprouted from the cracked asphalt, casting an eerie, pulsating green and purple glow onto the decaying facades of skeletal skyscrapers. A gentle, constant rain creates shimmering reflections in the puddles below, and the only sounds are the soft patter of rain and a low, otherworldly hum from the glowing fungi.`

### Sample 19 - Iridescent Moon-Dust Plain
- Prompt style family: `sci-fi-fantasy` with `landscape-environment` secondary
- Use case: Sci-fi films, alien worlds, fantasy landscapes
- Sample prompt: `A snow-covered plain of iridescent moon-dust under twilight skies. The surface shimmers with ethereal colors as camera slowly pans across the alien landscape. Otherworldly ambient sounds create an atmospheric soundscape. Sci-fi cinematic aesthetic.`

### Sample 20 - Off-Road Rally
- Prompt style family: `action-dynamic`
- Use case: Extreme sports, action sequences, racing content
- Sample prompt: `The scene explodes with the raw, visceral energy of a hardcore off-road rally, captured with a dynamic, almost found-footage aesthetic. The camera is shaky, seemingly mounted inside one of the vehicles, frequently splattered with mud. Several heavily modified off-road vehicles engage in a frenetic race through dense, muddy forest trails. Engine roars, mud splashing, and radio chatter create intense audio. Action sports documentary style.`

### Sample 21 - Modern Home Walkthrough
- Prompt style family: `real-estate-architecture`
- Use case: Real estate marketing, architecture portfolios, property tours
- Sample prompt: `The camera glides smoothly through a modern architectural home starting from the grand entrance hall. Floor-to-ceiling windows flood each room with natural daylight. Smooth gimbal movement carries the viewer through living space to kitchen to bedroom. Soft footsteps on hardwood floors with subtle ambient music. Elegant and unhurried pacing. High-end real estate style.`

### Sample 22 - Street Market Evening
- Prompt style family: `landscape-environment` with `social-viral` secondary
- Use case: Travel content, cultural documentaries, lifestyle videos
- Sample prompt: `The view moves through a busy street market at dusk as vendors begin turning on their lights. Camera glides naturally through the crowd at eye level. Colorful products, hanging lanterns, and busy vendor stalls fill the frame. Layered sounds: vendors calling out, music from shops, conversations in different languages. Vibrant and authentic atmosphere.`

### Sample 23 - Cluttered Desk Transformation
- Prompt style family: `transformation-timelapse`
- Use case: Organizing content, satisfying videos, productivity tips
- Sample prompt: `Split screen timelapse shows a cluttered home office transforming into an immaculately organized workspace. Camera maintains static wide angle throughout. Items disappear, surfaces get cleaned, organization systems appear in fast motion. Bright overhead lighting. Fast-paced satisfying music plays. Occasional sounds: boxes closing, papers filing, drawers shutting.`

### Sample 24 - Dancer Preparation
- Prompt style family: `performance-artistic`
- Use case: Dance videos, performance art, emotional storytelling
- Sample prompt: `Extreme close-up on a dancer's eyes as she takes a deep breath before performing. Dramatic side lighting creates strong contrast on her face. Camera holds steady as emotions shift: nervousness to determination to confidence. Shallow depth of field keeps background completely blurred. Her breathing is the only sound for several seconds before music begins faintly. Artistic performance style.`

### Sample 25 - Social Media Selfie
- Prompt style family: `social-viral`
- Use case: Social media content, vlogs, relatable commentary
- Sample prompt: `Selfie-style video of a person in their apartment holding phone with arm extended naturally. Natural lighting from large window creates soft shadows. They look directly into camera with slightly conspiratorial expression and say: "Nobody talks about how productivity advice is just procrastination with better marketing." Background sounds of city traffic and casual apartment ambiance. Relatable vlog aesthetic. No subtitles.`
