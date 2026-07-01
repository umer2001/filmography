# Veo Prompting Principles

## Purpose

This note distills practical prompt-generation lessons for Filmography from the local Veo 3.1 prompt guide at `/home/umer2001/projects/filmography/www.imagine.art_blogs_veo-3-1-prompt-guide.2026-06-30T11_05_12.588Z.md`.

Use this as a compact internal reference when improving shot-generation, reference-planning, sound-design, or prompt-generation behavior.

## Core Formula

Strong Veo prompts usually include:

`[Shot Composition] + [Subject Details] + [Action] + [Setting/Environment] + [Aesthetics/Mood] + [Audio]`

For Filmography, this maps to:
- shot composition: framing, camera angle, camera movement, lens feel, shot size
- subject details: character, object, product, food, performer, environment, wardrobe, prop state
- action: visible behavior, transformation, timed beat, interaction, dialogue moment
- setting/environment: place, time, weather, spatial markers, world rules
- aesthetics/mood: realism level, palette, lighting, texture, genre feel, emotional tone
- audio: dialogue, ambience, effects, silence, music, timing, no-subtitle instruction

## Prompt Style Families

Use the shot's practical purpose to choose prompt style:
- `cinematic-atmospheric`: emotional realism, mood, intimacy, suspense, melancholy, establishing atmosphere
- `character-dialogue`: speaking characters, performance, subtext, reaction timing, locked dialogue
- `professional-business`: workplace, training, explainer, corporate, instructional content
- `product-showcase`: e-commerce, object reveal, feature montage, assembly, tactile prop clarity
- `culinary-food`: cooking, food prep, cafe, restaurant, tactile food detail
- `landscape-environment`: travel, nature, city, weather, aerial, environment-led b-roll
- `stylized-creative`: anime, period, vintage, surreal, graphic, art-directed looks
- `sci-fi-fantasy`: speculative worlds, magical environments, futuristic or otherworldly settings
- `action-dynamic`: sports, chase, rally, handheld energy, fast physical movement
- `real-estate-architecture`: property walkthroughs, interiors, architecture, spatial flow
- `transformation-timelapse`: before/after, process, cleanup, construction, growth, time compression
- `performance-artistic`: dance, music, stage, artistic preparation, expressive body movement
- `social-viral`: selfie, vlog, direct-to-camera, relatable short-form speech

## Selection Rule

Classify by the shot's use case, not only by the overall scene genre. A quiet drama can still contain:
- a `product-showcase` prop insert when an object is story proof
- a `character-dialogue` reaction shot when silence or a line carries the beat
- a `landscape-environment` establishing shot when the location or weather is the subject
- a `transformation-timelapse` shot when visible change over time matters

## Audio Rules

Veo prompt sheets should explicitly carry audio when it matters:
- locked dialogue verbatim
- ambience bed
- precise sound cues
- timing for pauses, beats, and line delivery
- silence or near-silence when it is emotionally important
- `No subtitles` when text overlays are unwanted

## Reference Rules

Use references to reduce drift:
- character references for dialogue, performance, wardrobe, expression, and identity
- prop/product references for object inserts and detail-dependent shots
- environment/style frames for atmosphere-heavy or stylized scenes
- start/end or bridge frames for stitched movement, transformations, and continuity-sensitive blocking

## Quality Gate

Before finalizing a Veo prompt, confirm:
- camera/framing/movement are explicit
- subject or object identity is anchored
- visible action is clear
- setting/environment is stable
- aesthetics and mood are bounded
- audio is explicit
- references are named where mandatory
- negative constraints target likely drift
- stitched shots include motion bridge and carry-over continuity
- timestamped sequences include beat timing

## Sample Prompt Library

Use these as style references when selecting prompt families for new shots. They show how different use cases shape camera, subject, action, setting, aesthetics, and audio.

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
