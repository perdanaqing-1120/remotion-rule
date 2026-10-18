Master AI System Rules: Remotion Unified Hybrid Engine (`rule.md` - v9 Pure English Edition)
This document serves as the Single Source of Truth (Master Architectural Specification) for AI when generating Remotion (React + TypeScript) video code. All rules in this specification focus strictly on spatial layout, coordinates, motion physics, camera rigs, color palettes, UI micro-interactions, scene transitions, and ElevenLabs audio-visual synchronization—independent of the subject matter or spoken language.
> **CORE PRINCIPLE — UNIFIED MULTI-STYLE ORCHESTRATION (NO MODE LOCKING):**
> The AI is **STRICTLY PROHIBITED** from locking an entire video into a single static visual style or mode. Every component, 2.5D/3D camera rig, kinetic typography pattern, dark glassmorphic surface, tactile paper cutout, brutalist card, and technical HUD element in this specification belongs to **One Unified Ecosystem**. The AI **MUST dynamically combine and alternate these patterns from scene to scene** (and layer them harmoniously within compositions) so the video remains visually engaging, varied, and structurally coherent at all times.
---
PART I: AI NARRATIVE-TO-VISUAL ROUTER (DIRECTIONAL COMPASS)
To ensure the AI never loses direction when converting a script into a Remotion video, the AI MUST map each sentence or narrative beat using the orchestration matrix below:
1. The Anti-Monotony Rule (3-Second Visual Shift Rule)
Mandatory Visual Pattern Shift Every 2.5 – 4.0 Seconds (`75 – 120 Frames` @30fps):
Never use the exact same layout structure or component archetype in two consecutive scenes.
If Scene A uses Centered Kinetic Typography, Scene B must shift to 3D Device Pop-Out / Bento Grid / Cutout Sticker Collage / Interactive Diagram, and Scene C must shift to Vertical Whip-Scroll Carousel / 3D Perspective Card / Split Comparison.
Narrative-to-Visual Mapping Matrix (Mandatory Scene Selection Guide):
Narrative Function in Script	Mandatory Visual & Component Combination	Entry Transition Archetype
1. Opening Hook / Surprise Question	`<HalftoneCutoutSticker />` + `<DynamicFlexTextWithPill />` + `<HighlightStrip />` OR `<RadialIrisTransition />` + `<WireframeEchoHeadline />`	Radial Iris Expansion (`5f`) or 3D Device/Sticker Pop-In (`12f`)
2. Naming / Code / Acronym Breakdown	Tokenized Typography (split into individual `<span>` tokens, highlight active token with accent color, dim inactive tokens to `opacity: 0.25`) + `<TokenCalloutCards />` (animated SVG Bezier curves) OR `<AcronymVerticalBreakdown />`	Gaussian Blur Dissolve (`9f`) or Layout Morphing
3. App Showcase / Product Proof / OS	`<Device3DPopOutRig />` (tilted 3D phone/PC detaching floating UI cards toward the camera) OR `<RetroWarningModal />` + `<HandDrawnAnnotation />`	Camera Dolly-In + Card Detachment (`11f`) or Horizontal Whip-Pan (`9f`)
4. Expense / Item List / History Feed	`<PinnedCounterCarousel />` (live incrementing/decrementing header counter pinned at top + Vertical Whip-Scroll List below)	Vertical Whip-Scroll (`20–22f`, `Easing.bezier(0.22, 1, 0.36, 1)`)
5. Step-by-Step Workflow (`#1, #2, #3`)	`<StampStepBadge />` at top-left + Rotating Tactile Paper Canvas + `<RetroTVCodePreview />` / `<InteractivePromptCanvas />`	Paper Wash Cross-Fade (`6–9f`) + Bouncy Spring Pop-In
6. Hardware / Silicon / Audio / AI Core	Automatic transition into Deep Dark Canvas + `<HardwareDieDiagram />` (camera zoom into glowing silicon block) OR `<AudioWaveformCloneComparison />` / `<ClientServerFlow />`	Contextual Dark Fade (`10f`) + Camera Zoom-In (`scale: 1 -> 1.2`)
7. Multi-Metric Data / Statistics Recap	`<SynchronizedBentoDashboard />` (4–5 cards animating simultaneously: SVG line chart, donut chart, toggle switch, equalizer, keyframe track) OR `<SpecSheetCard />` + `<MagnifyingGlassScanner />`	Staggered Grid Scale-In (`3f` delay per card)
8. Input Simulation / Calculator / CLI	`<BentoFormCameraRig />` (2-column input grid with vertical camera pan + active green border & blinking cursor `	`) OR `<LiveCodeTerminal />`
9. Emotional Climax / Visual Art / Music	`<Parallax3DTextSandwich />` (giant headline sandwiched between foreground and background 3D iridescent objects) OR `<Perspective3DMusicCard />` + `<NeonBloomHeadline />`	1-Frame White Flash Cut or Dramatic Blackout Pause (`15f`)
10. Call-to-Action (CTA) / Outro	`<HorizontalWhipCTAWithCursor />` (2-word statement whipped left to reveal pill CTA button + pointer click) -> `<OrbitalIdentityLockup />` / `<CommentSimulationCTA />`	Horizontal Whip-Pan (`10f`) + Pointer Button Press (`scale: 0.93`)
---
PART II: SPATIAL ARCHITECTURE, Z-DEPTH LAYERING, & CANVAS SAFE-ZONES
To ensure that combining multiple visual styles always looks cohesive, clean, and uncluttered, the AI must enforce the following spatial hierarchy on every frame:
1. The 4-Layer Z-Depth Architecture (`<AbsoluteFill>` Stack)
Every Remotion composition must be structured into 4 distinct `<AbsoluteFill>` depth layers from back to front:
Layer 0 — Dynamic Canvas & Atmospheric Texture (`zIndex: 0`):
Contains the base canvas background color (which may transition across scenes), Ambient Radial Glows (`filter: blur(140px)`), subtle Tactile Paper Noise (`feTurbulence`, `opacity: 0.05`), and soft inner vignette shading.
Layer 1 — Secondary Context / Blurred Background (`zIndex: 10`):
When a foreground modal card, summary pop-up, or focal statement appears, do not immediately unmount the previous scene's context object. Retain the background object (e.g., 3D device mockup, Bento input grid, or storyboard matrix) in Layer 1 with `filter: blur(10px) brightness(0.45)` and `transform: scale(0.94)` to create optical Depth of Field.
Layer 2 — Main Focal Stage (`zIndex: 20`):
The primary visual stage in the center of the canvas. Single Focal Point Rule: Only 1 primary visual concept group may occupy Layer 2 at any given moment, preserving at least 45–50% open whitespace.
When using a 3D Depth Sandwich, subdivide Layer 2 into:
`Sub-Layer 2A (Background Objects, zIndex: 18)`: Iridescent spheres, particle fields, or parallax clouds.
`Sub-Layer 2B (Midground Typography, zIndex: 20)`: Giant headline text or primary hero card.
`Sub-Layer 2C (Foreground Objects, zIndex: 22)`: Dichroic glass capsule, cutout sticker, or magnifying loupe passing directly in front of the text.
Layer 3 — Persistent Chrome, HUD, & Subtitle Safe-Zone (`zIndex: 100`):
Structural anchor elements locked to the perimeter of the canvas:
Top Header Option (`top: 60..140px`): Constant Brand Logo + dynamic Context Pill Badge (`#111111` capsule or perforated stamp badge) or Pinned Live Counter Header.
Technical HUD Option (`padding: 36px`): 4 corner brackets (`18x18px`, `1px solid`), Live Timecode (`TC 00:00:SS:FF`) at top-right, and Bottom Ruler Progress Bar (`01 / KINETIC TYPE`) using `mixBlendMode: 'difference'`.
Bottom Subtitle & Watermark Zone (`bottom: 120..260px`): Static creator handle `@handle` (`opacity: 0.35`) positioned directly above the Dynamic Karaoke Subtitle (maximum 3–5 words per phrase).
---
PART III: CHAMELEON COLOR SYSTEM (ADAPTIVE PALETTES)
The AI may transition between the palettes below across scenes (using Radial Iris, Paper Wash Cross-Fade, or Staccato Beat Cuts), but within any single scene, the AI must strictly pair surface and accent colors from the active palette to guarantee high contrast:
1. Palette A: Dark Glassmorphism & Cosmic Tech (For SaaS UI, Silicon Breakdown, Audio, & 3D Depth)
Deep Canvas Backgrounds: `#0A150A` (Obsidian Forest Black), `#0D0D0F` (Carbon Black), or `#121024` (Deep Cosmic Indigo).
Ambient Radial Glows: `#0D3810` (Emerald Glow at top-left `cx: 15%, cy: 18%`) + `#261808` (Warm Amber Glow at bottom-right `cx: 82%, cy: 78%`).
Elevated Glass Card Surface: `#17181D` (`backdropFilter: blur(20px)`, `border: 1px solid rgba(255,255,255,0.09)`, `boxShadow: 0 24px 60px rgba(0,0,0,0.65)`).
Secondary Sub-Item Card: `#121514` (`border: 1px solid rgba(255,255,255,0.06)`).
Semantic Accents: Neon Green `#22C55E` (Primary CTA, positive delta, active input focus ring), Vermilion Orange `#EA580C` (Hardware/NPU highlight, active playhead), Electric Violet `#4F39F6` (Keyframe track, geometric tiles), Acid Lime `#B8E92E` (Rhythm meter, active state).
2. Palette B: Tactile Editorial & Clean Explainer (For Concepts, Workflows, Cutout Collages, & Light Bento)
Rotating Paper & Light Canvases:
Warm Alabaster / Off-White Paper: `#EAE6DF` / `#F6F6F7` / `#DBD7D0`
Mustard Yellow Paper: `#DEC658`
Dusty Rose / Mauve Pink Paper: `#CFA1AE`
Deep Forest Green Paper: `#143B27`
Vermilion Red-Orange Paper: `#D4421E` / `#E2451D`
Cobalt Royal Blue Paper: `#1B3AC4`
Card Surfaces on Light Canvases:
Clean Floating Card: `#FFFFFF` with `border: 1.5px solid rgba(0,0,0,0.06)` and `boxShadow: 0 16px 40px rgba(0,0,0,0.05)`.
Brutalist Neo-Retro Card: `#F3F2EE` with `border: 3px solid #111111` and hard offset shadow `boxShadow: 8px 8px 0px #111111`.
Highlight Strip Contrast Rule (`<HighlightStrip />`):
Use a Vermilion Red-Orange strip (`#D94622`) with `#FFFFFF` text across all canvas colors, EXCEPT when the canvas background itself is Red-Orange (`#D4421E` / `#E2451D`), in which case the highlight strip must automatically switch to Jet Black (`#111111`).
---
PART IV: MASTER COMPONENT CATALOG & OBJECT CHOREOGRAPHY (MIX-AND-MATCH)
The AI has unrestricted access to all components below and should assemble them dynamically based on narrative intent:
1. Kinetic Typography & Text Deconstruction Components
Tokenized Product/Concept Title (`<TokenizedTitle />`):
Never render multi-part names or codes as a single static text string. Split every word/number into an independent `<span style={{ display: 'inline-flex' }}>`.
When explaining a specific token, dim inactive tokens to `opacity: 0.25`, highlight the active token in `#EA580C` or `#22C55E`, and draw an animated SVG Bezier curve (`strokeDasharray` + `strokeDashoffset`) from the bottom center of the active token to its explanation card below.
Support Layout Morphing (animating a badge token like `HX` from the end of a string to the middle using `translateX/Y`) and `<MissingSlot />` (`border: 3px dashed #EA580C`, `borderRadius: 14px` containing a blinking `?` or `empty` label).
Dynamic Flex Push with Inline Pill (`<DynamicFlexTextWithPill />`):
Centered single-line flex container (`display: 'flex'`, `alignItems: 'center'`, `justifyContent: 'center'`, `gap: 16`).
When an inline pill badge (`border: 1px solid #22C55E`, `background: rgba(34,197,94,0.12)`, `borderRadius: 999px`) expands in the middle or right of the sentence, animate its `maxWidth` from `0px` to `260px` using `spring()`, smoothly pushing the preceding words to the left without layout jumps.
Mixed Editorial Typography + Animated Highlight Strip (`<EditorialHeadline />`):
Combine Medium Sans-Serif (`Inter` / `Plus Jakarta Sans` on line 1), Bold Italic Editorial Serif (`Playfair Display` / `Instrument Serif` on line 2), and Extra-Bold Sans-Serif mounted inside an animated `<HighlightStrip />` (`scaleX: 0 -> 1`, `transformOrigin: 'left'`, `rotate: -1deg`) on line 3.
Wireframe Echo & Wave-Distorted Typography (`<WireframeEchoHeadline />` & `<WavyKineticWord />`):
Render 2–3 duplicate outline layers (`fill: 'none'`, `strokeWidth: 1`, `opacity: 0.25`) that converge toward `(0, 0)` as the main headline settles, or apply SVG wave distortion (`<feDisplacementMap>` / sinusoidal `<textPath>`) accented by rotating 4-point concave stars (`✦`).
2. UI Cards, 3D Device Mockups, & Bento Dashboard Components
3D Isometric Device Pop-Out Rig (`<Device3DPopOutRig />`):
Initialize the device container in 3D space (`perspective: 1200px`, `rotateX(12deg) rotateY(-18deg) rotateZ(14deg)`).
Over `11 frames` (@30fps), interpolate device rotation to `0deg`, scale the device up (`1.0 -> 1.45`), and blur it into the background (`blur: 0 -> 14px`, `opacity: 0.35`), while detaching the primary Hero Summary Card forward (`scale: 0.42 -> 1.0`) followed by a staggered cascade of 3 sub-item cards below (`3f` delay per card, descending opacity `1.0`, `0.75`, `0.45`).
Pinned Header Counter + Vertical Whip-Scroll Carousel (`<PinnedCounterCarousel />`):
Lock a Sticky Header Bar at the top of the frame featuring a live incrementing/decrementing number counter on the right (`interpolate`).
Below the header, wrap category card groups inside a vertically masked viewport (`maskImage: 'linear-gradient(to bottom, transparent 0%, black 12%, black 85%, transparent 100%)'`) that scrolls upward in `22-frame` (@30fps) cycles using `Easing.bezier(0.22, 1, 0.36, 1)`.
Synchronized Multi-Card Bento Dashboard (`<SynchronizedBentoDashboard />`):
Arrange 4–5 distinct cards (White `#FFFFFF`, Vermilion `#F04E23`, Carbon Black `#141416`, Acid Lime `#B8E92E`, Electric Violet `#5238F2`) in a unified CSS Grid.
Trigger all internal card micro-animations simultaneously over a `60-frame` window: live percentage counter (`+201% -> +248%`), rising SVG Bezier curve, sliding toggle switch, circular donut gauge (`4% -> 99%`), bouncing 7-bar BPM equalizer, orange timeline playhead sweeping across lime diamond keyframes, and a pointer cursor clicking a pill button from `RENDER` (white) to `DONE` (lime green).
2-Column Bento Form Camera Rig (`<BentoFormCameraRig />`):
A 2-column grid of input cards panning upward (`translateY: +180px -> -140px`) as the virtual camera moves down toward a full-width neon green CTA button. Active input cards illuminate with `border: 1.5px solid #22C55E`, sequential typewriter character slicing, and a blinking vertical cursor (`|`).
Perspective 3D Scrolling Lyric/Item Card (`<Perspective3DMusicCard />`):
A rounded dark card floating in 3D perspective (`rotateX(14deg) rotateY(-18deg) rotateZ(6deg)`) where the active line is crisp white (`blur(0px), opacity: 1, scale: 1.05`) while preceding and upcoming lines are optically defocused (`blur(3.5px), opacity: 0.35, scale: 0.96`).
3. Tactile Cutout Stickers, Retro OS, & Interactive Preview Components
Halftone Cutout Sticker & Torn Paper Frame (`<HalftoneCutoutSticker />`):
Apply high-contrast monochrome/vintage grading to subject cutouts (people, lightbulbs, typewriters, CRT TVs, vintage PCs, microphones, stopwatches) surrounded by a thick, irregular white paper die-cut border (multi-directional `drop-shadow` in `#F4F1EA` at `10px–14px` plus soft ambient shadow `rgba(0,0,0,0.28)`).
Interactive Prompt-to-Canvas Preview (`<InteractivePromptCanvas />`):
Display a central preview card (`border: 3px solid #111111`, `boxShadow: '8px 8px 0px #111111'`) paired with a dark chat prompt bubble at the top-right. On the exact frame the prompt bubble pops in, mutate the target property inside the preview card (e.g., text `scale` jumps `1.0 -> 1.85` via `bouncy` spring or card background switches to `#D94622`).
Storyboard Grid with Magnifying Loupe (`<StoryboardGridWithLoupe />`):
A `6x3` matrix of miniature vertical scene cards labeled with monospace timestamps (`0.0s`, `2.5s`) scanned by a red-orange playhead line and a floating `<MagnifyingLoupe />` that scales up the underlying cards (`scale: 1.35`) inside its circular glass lens.
Retro OS Warning Modal & Hand-Drawn Marker (`<RetroWarningModal />`):
Classic blue-header OS dialog (`[-] [□] [X]`) paired with zig-zag tilted word strips (`<TiltedWordPills />`), a real-time hand-drawn red marker circle (`strokeDashoffset`), and a green checkmark (`✓`).
4. Technical Gauges, Silicon Diagrams, & High-Conversion CTA Components
Arc Speedometer, Power Bar & Stamp Overlay (`<ArcGauge />` & `<StampOverlay />`):
Half-circle SVG gauge (`strokeLinecap="round"`, `strokeWidth={24}`) with a `spring()` rotating needle (`-75deg` to `+75deg`), an incrementing wattage/power bar, and a tilted red warning stamp (`rotate(-8deg)`) slamming down from `scale: 2.2` to `1.0`.
Hardware Die, Audio Waveform, & Client-Server Flow (`<HardwareDieDiagram />` & `<AudioWaveformCloneComparison />`):
Internal chip schematic where the target block (`NPU`) glows bright orange (`boxShadow: '0 0 45px rgba(234,88,12,0.6)'`) during a camera zoom-in; dual synchronized audio waveforms (white original voice top vs. red-orange cloned voice bottom); and animated data packets flowing along a dashed vertical line between Server and Laptop.
Horizontal Whip-Pan CTA with Cursor Click (`<HorizontalWhipCTAWithCursor />`):
Display a punchy 2-word statement in the center, then whip the camera left (`translateX: 0 -> -580px` over `10 frames` @30fps) leaving `10–15%` of the trailing letters visible at the left edge while a neon green pill button enters center stage and is clicked by an animated hand cursor (`scale: 1 -> 0.93 -> 1.0`).
Orbital Identity Lockup & Comment Simulation (`<OrbitalIdentityLockup />` & `<CommentSimulationCTA />`):
Finale lockup featuring a per-character wave-spring headline encircled by tilted 3D elliptical comet orbits (dynamically toggling `zIndex` between `+10` in front of text and `-10` behind text), or an automated typewriter comment input box with an instant admin reply card.
---
PART V: FRAME-ACCURATE TRANSITION TIMINGS & MOTION PHYSICS LOOKUP
All transition durations and motion vectors below are derived from frame-by-frame optical flow measurements and MUST be used by the AI when coding `interpolate()` and `spring()` animations:
Transition / Motion Archetype	Exact Duration (@30fps / @60fps)	Vector Mechanics & Easing Curve in Remotion
1. Radial Iris Expansion	`5 Frames` (`0.167s`) / `10 Frames`	Center circle at `(50%, 50%)` expands from `scale(0)` to `scale(28)` using `Easing.bezier(0.7, 0, 0.15, 1)` to fill `100%` of the viewport.
2. 3D Device to UI Card Pop-Out	`11 Frames` (`0.367s`) / `22 Frames`	3D device straightens to `0deg`, `scale(1 -> 1.45)`, `blur(0 -> 14px)`, while the hero card detaches forward (`scale: 0.42 -> 1.0`) followed by a 3-card cascade (`3f` stagger).
3. UI Stack to Center Text Crossover	`9 Frames` (`0.300s`) / `18 Frames`	5f Exit: UI stack shrinks (`scale: 0.88`), rises (`dy = -5 px/f`), `blur(16px)`, `opacity(0)`. 1f Crossover. 4f Enter: Center text rises (`Y: 317 -> 296px`) and sharpens (`blur: 10px -> 0px`).
4. Horizontal Whip-Pan (Overlapping)	`8–10 Frames` (`0.30s`) / `16–20 Frames`	Outgoing scene whips left (`dx = -52 to -65 px/f`) with directional stretch (`scaleX: 1.35`) and `<feGaussianBlur>`. Incoming scene enters from the right edge on the final `10%` overlap frame.
5. Vertical Whip-Scroll Carousel	`22 Frames` (`0.733s`) / `44 Frames`	Outgoing card group accelerates upward (peak `dy = -30 px/f`) through the top gradient mask while the incoming group rises from below via `Easing.bezier(0.22, 1, 0.36, 1)`.
6. Paper Wash / Texture Cross-Fade	`6–9 Frames` (`0.25s`) / `12–18 Frames`	Paper background color cross-fades with a brief `contrast(1.3)` pulse while cutout stickers enter/exit using the `bouncy` spring preset.
7. Staccato Beat / Flash Cut	`3–7 Frames` (`0.10–0.23s`) / `6–14 Frames`	Rapid rhythmic cuts synced to audio beats, or a 1-Frame White Flash (`#FFF8F3`) decaying exponentially over `6–10 frames` into a 3D or climax scene.
8. Standard UI `spring()` Presets	`12–18 Frames` / `24–36 Frames`	`snappy`: `{ mass: 0.8, damping: 16, stiffness: 180 }` (Cards, Modals, Text Strips).<br>`bouncy`: `{ mass: 0.6, damping: 10, stiffness: 240 }` (Stickers, Badges, Stamps, Clicks).<br>`smooth`: `{ mass: 1.0, damping: 24, stiffness: 120 }` (2.5D/3D Camera Rigs & Panning).
---
PART VI: MANDATORY ELEVENLABS VOICEOVER & AUDIO-VISUAL SYNCHRONIZATION
The AI must use ElevenLabs as the primary voiceover engine (Text-to-Speech) and bind all scene cuts, text highlights, and object animation triggers directly to the word-level timestamps returned by ElevenLabs.
Pre-Render Generation Script via `with-timestamps` Endpoint (`scripts/generate-voice.ts`):
Execute a pre-render Node.js script calling `POST https://api.elevenlabs.io/v1/text-to-speech/{voice_id}/with-timestamps` with model `eleven_multilingual_v2` (or `eleven_turbo_v2_5`) and voice settings `{ stability: 0.55, similarity_boost: 0.80, style: 0.25, use_speaker_boost: true }`.
Decode the Base64 audio stream into `public/audio/voiceover.mp3` and convert the character-level `alignment` arrays (`characters`, `character_start_times_seconds`, `character_end_times_seconds`) into word-level timestamp objects (`word`, `start`, `end`, `startFrame`, `endFrame`) saved to `src/data/voice-timestamps.json`.
Dynamic Composition Duration & Frame-Accurate Visual Triggers:
Use `calculateMetadata` in `Root.tsx` so that `durationInFrames = Math.ceil((audioDurationInSeconds + 1.5) * fps)`.
Trigger every major component entry, `<DynamicFlexTextWithPill />` expansion, `<HighlightStrip />` wipe, `<ArcGauge />` sweep, and `<PinnedCounterCarousel />` scroll cycle using `<Sequence from={word.startFrame}>` mapped to the exact keyword in `voice-timestamps.json`.
Illuminate each word in headlines and karaoke subtitles from dim (`opacity: 0.25`) to active (`opacity: 1.0`) precisely when `currentTime >= word.start`.
Audio Mounting & Automatic Background Music Ducking:
Mount `<Audio src={staticFile('audio/voiceover.mp3')} volume={1.0} />` at the root `<AbsoluteFill>`, and apply automatic Audio Ducking to any background music track (`volume: 0.14` while ElevenLabs voiceover words are active, ramping up to `0.40` during transition pauses and the outro).
