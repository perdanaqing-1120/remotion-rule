Master AI System Rules: Remotion Unified Hybrid Engine (`rule.md` - v8)
Dokumen ini adalah Single Source of Truth (Panduan Arsitektur Utama) bagi AI saat men-generate kode video Remotion (React + TypeScript).
> \*\*PRINSIP UTAMA — TANPA BATASAN MODE (UNIFIED MULTI-STYLE ORCHESTRATION):\*\*
> AI \*\*DILARANG\*\* mengunci diri hanya pada satu gaya/mode tunggal di sepanjang video. Seluruh katalog komponen, kamera 2.5D/3D, \*kinetic typography\*, \*dark glassmorphism\*, \*tactile paper cutout\*, \*brutalist card\*, hingga \*technical HUD\* di dalam dokumen ini adalah \*\*Satu Ekosistem Terpadu\*\* yang \*\*WAJIB dikombinasikan secara dinamis dari scene ke scene\*\* (bahkan dilapiskan secara harmonis dalam satu komposisi) agar video selalu hidup, variatif, dan \*\*AI tidak pernah kehilangan arah\*\*.
---
BAGIAN I: KOMPAS PENGARAH AI (NARRATIVE-TO-VISUAL ROUTER)
Agar AI tidak pernah bingung atau kehilangan arah saat mengubah naskah menjadi video Remotion, AI WAJIB memetakan setiap kalimat/ketukan narasi menggunakan matriks orkestrasi di bawah ini:
1. Aturan Anti-Monoton (The 3-Second Visual Shift Rule)
Pergantian Pola Visual Tiap 2.5 – 4.0 Detik (`75 – 120 Frame` @30fps):
Jangan pernah menggunakan jenis tata letak atau komponen yang sama pada dua scene berturut-turut.
Jika Scene A menggunakan Tipografi Kinetik, maka Scene B wajib beralih ke Kartu UI / Bento Grid / Stiker Kolase / Diagram Interaktif, lalu Scene C beralih ke 3D Perspective / Carousel Scroll / Split Comparison.
Matriks Pemetaan Narasi ke Visual (Wajib Diikuti AI untuk Setiap Kalimat):
Fungsi Kalimat dalam Naskah	Kombinasi Visual & Komponen yang WAJIB Dipilih AI	Transisi Masuk yang Digunakan
1. Hook Pembuka / Pertanyaan Kejutan	`<HalftoneCutoutSticker />` + `<DynamicFlexTextWithPill />` + `<HighlightStrip />` ATAU `<RadialIrisTransition />` + `<WireframeEchoHeadline />`	Radial Iris Expansion (`5f`) atau 3D Device/Sticker Pop-In (`12f`)
2. Penjelasan Nama / Kode / Singkatan	Tokenized Typography (pecah per `<span>`, sorot warna aksen, redupkan sisanya `opacity: 0.25`) + `<TokenCalloutCards />` (garis kurva Bezier SVG) ATAU `<AcronymVerticalBreakdown />`	Gaussian Blur Dissolve (`9f`) atau Layout Morphing
3. Pameran Aplikasi / Bukti Produk / OS	`<Device3DPopOutRig />` (HP/PC 3D miring yang melepaskan kartu UI ke depan layar) ATAU `<RetroWarningModal />` + `<HandDrawnAnnotation />`	Camera Dolly-In + Card Detachment (`11f`) atau Horizontal Whip-Pan (`9f`)
4. Rincian Biaya / Daftar Item / Riwayat	`<PinnedCounterCarousel />` (Header angka berhitung mundur/naik secara live di atas + Vertical Whip-Scroll List di bawah)	Vertical Whip-Scroll (`20–22f`, `Easing.bezier(0.22, 1, 0.36, 1)`)
5. Bedah Alur Kerja / Langkah (`#1, #2, #3`)	`<StampStepBadge />` di pojok kiri-atas + Rotasi Kanvas Kertas Bertekstur + `<RetroTVCodePreview />` / `<InteractivePromptCanvas />`	Paper Wash Cross-Fade (`6–9f`) + Bouncy Spring Pop-In
6. Bedah Hardware / Prosesor / Suara / AI	Latar otomatis masuk ke Deep Dark Canvas + `<HardwareDieDiagram />` (zoom ke chip menyala) ATAU `<AudioWaveformCloneComparison />` / `<ClientServerFlow />`	Contextual Dark Fade (`10f`) + Camera Zoom-In (`scale: 1 -> 1.2`)
7. Ringkasan Data / Statistik Multi-Metrik	`<SynchronizedBentoDashboard />` (4–5 kartu berjalan serempak: grafik kurva, donut chart, toggle, equalizer, keyframe) ATAU `<SpecSheetCard />` + `<MagnifyingGlassScanner />`	Staggered Grid Scale-In (`3f` jeda antar-kartu)
8. Simulasi Input / Kalkulator / Koding	`<BentoFormCameraRig />` (Grid 2 kolom dengan kamera pan vertikal + ketikan berkursor `	`) ATAU `<LiveCodeTerminal />`
9. Klimaks Emosional / Visual Art / Musik	`<Parallax3DTextSandwich />` (Teks raksasa diapit objek 3D iridescent depan-belakang) ATAU `<Perspective3DMusicCard />` + `<NeonBloomHeadline />`	1-Frame White Flash Cut atau Dramatic Blackout Pause (`15f`)
10. Call-to-Action (CTA) / Penutup (Outro)	`<HorizontalWhipCTAWithCursor />` (Teks 2 kata dibanting ke kiri membuka tombol kapsul + klik kursor tangan) $	
ightarrow$ `<OrbitalIdentityLockup />` / `<CommentSimulationCTA />`	Horizontal Whip-Pan (`10f`) + Pointer Button Press (`scale: 0.93`)	
---
BAGIAN II: ARSITEKTUR SPASIAL, LAPISAN Z-DEPTH, & TATA LETAK KANVAS
Agar penggabungan berbagai gaya visual tetap terlihat rapi, berkelas, dan tidak pernah berantakan (cluttered), AI wajib mematuhi aturan ruang berikut pada setiap frame:
1. Aturan 4 Lapisan Kedalaman (`Z-Index Layering Architecture`)
Setiap komposisi Remotion wajib disusun menggunakan 4 lapisan `<AbsoluteFill>` dari belakang ke depan:
Layer 0 — Dynamic Canvas & Atmospheric Texture (`zIndex: 0`):
Berisi warna dasar kanvas (yang dapat berganti antar-scene), Ambient Radial Glows (`filter: blur(140px)`), serta tekstur halus Tactile Paper Noise (`feTurbulence`, `opacity: 0.05`) dan inner vignette.
Layer 1 — Secondary Context / Blurred Background (`zIndex: 10`):
Saat sebuah kartu modal, pop-up, atau teks kesimpulan muncul di depan, jangan langsung menghapus objek dari detik sebelumnya. Pertahankan objek sebelumnya (seperti mockup HP 3D, tabel form, atau grid storyboard) di Layer 1 dengan `filter: blur(10px) brightness(0.45)` dan `transform: scale(0.94)` untuk menciptakan Optical Depth of Field.
Layer 2 — Main Focal Stage (`zIndex: 20`):
Panggung utama di tengah layar. Aturan Single Focal Point: Hanya boleh ada 1 kelompok konsep visual aktif di Layer 2 pada satu waktu dengan minimal 45–50% ruang kosong (whitespace).
Jika menggunakan teknik 3D Depth Sandwich, bagi Layer 2 menjadi:
`Sub-Layer 2A (Back Object, zIndex: 18)`: Bola krom / partikel / awan latar.
`Sub-Layer 2B (Mid Typography, zIndex: 20)`: Teks judul raksasa atau kartu utama.
`Sub-Layer 2C (Front Foreground Object, zIndex: 22)`: Objek kapsul kaca / stiker cutout / kaca pembesar yang melintas di depan teks.
Layer 3 — Persistent Chrome, HUD, & Subtitle Safe-Zone (`zIndex: 100`):
Elemen penunjuk struktur yang dikunci di tepi layar agar penonton selalu punya jangkar visual:
Opsi Header Atas (`top: 60..140px`): Logo Brand + Context Pill Badge hitam/kuning (`Part 4`, `LANGKAH #1`, atau Sticky Counter Header).
Opsi Frame Teknis (`padding: 36px`): 4 siku sudut (Corner Brackets), Live Timecode (`TC 00:00:SS:FF`), dan Bottom Ruler Progress Bar (`01 / KINETIC TYPE`) dengan `mixBlendMode: 'difference'`.
Zona Subtitle & Watermark Bawah (`bottom: 120..260px`): Watermark `@handle` (`opacity: 0.35`) + Dynamic Karaoke Subtitle (maksimal 3–5 kata per baris).
---
BAGIAN III: SISTEM PALET WARNA ADAPTIF (CHAMELEON COLOR SYSTEM)
AI dapat berpindah antar-tema warna di bawah ini secara dinamis saat berganti scene (menggunakan Radial Iris, Paper Wash, atau Hard Beat Cut), namun di dalam satu scene yang sama, AI wajib menggunakan pasangan warna yang sudah teruji kontrasnya:
1. Palet A: Dark Glassmorphism & Cosmic Tech (Untuk UI SaaS, Bedah Chip, Audio, & 3D Depth)
Deep Canvas: `#0A150A` (Obsidian Forest), `#0D0D0F` (Carbon Black), atau `#121024` (Cosmic Indigo).
Ambient Radial Glows: `#0D3810` (Emerald Glow di kiri-atas) + `#261808` (Amber Glow di kanan-bawah).
Elevated Glass Card: `#17181D` (`backdropFilter: blur(20px)`, `border: 1px solid rgba(255,255,255,0.09)`, `boxShadow: 0 24px 60px rgba(0,0,0,0.65)`).
Sub-Item Card: `#121514` (`border: 1px solid rgba(255,255,255,0.06)`).
Semantic Accents: Neon Green `#22C55E` (CTA/Positif/Fokus), Vermilion Orange `#EA580C` (Sorotan Chip/NPU/Playhead), Electric Violet `#4F39F6` (Timeline/Geometri), Acid Lime `#B8E92E` (Rhythm/Done).
2. Palet B: Tactile Editorial & Clean Explainer (Untuk Konsep, Langkah, Kolase, & Bento Terang)
Rotating Paper/Light Canvases:
Warm Alabaster / Off-White: `#EAE6DF` / `#F6F6F7` / `#DBD7D0`
Mustard Yellow: `#DEC658`
Dusty Rose Pink: `#CFA1AE`
Deep Forest Green: `#143B27`
Vermilion Red-Orange: `#D4421E` / `#E2451D`
Cobalt Royal Blue: `#1B3AC4`
Card Surfaces di Atas Latar Terang:
Clean Floating Card: `#FFFFFF` dengan `border: 1.5px solid rgba(0,0,0,0.06)` dan `boxShadow: 0 16px 40px rgba(0,0,0,0.05)`.
Brutalist Neo-Retro Card: `#F3F2EE` dengan `border: 3px solid #111111` dan bayangan blok keras `boxShadow: 8px 8px 0px #111111`.
Aturan Kontras Pita Sorotan (`<HighlightStrip />`):
Gunakan pita `#D94622` (Merah-Oranye) dengan teks `#FFFFFF` di atas semua warna latar, KECUALI saat latar kanvas berwarna Merah-Oranye (`#D4421E` / `#E2451D`), pita sorotan wajib otomatis berubah menjadi Hitam Pekat `#111111`.
---
BAGIAN IV: KATALOG MASTER KOMPONEN & KOREOGRAFI OBJEK (SEMUA DAPAT DIGABUNGKAN)
AI memiliki akses penuh ke seluruh komponen di bawah ini dan bebas merakitnya sesuai kebutuhan naskah:
1. Kelompok Komponen Tipografi Kinetik & Dekonstruksi Teks
Tokenized Product/Concept Text (`<TokenizedTitle />`):
Pecah setiap kata/angka penting menjadi `<span style={{ display: 'inline-flex' }}>` mandiri.
Saat menjelaskan satu bagian kode/kata, turunkan opasitas token lainnya menjadi `0.25`, sorot token aktif dengan warna aksen (`#EA580C` / `#22C55E`), dan tarik garis kurva Bezier SVG (`strokeDasharray` + `strokeDashoffset`) dari bawah token aktif menuju kartu penjelasannya.
Jika menjelaskan ketiadaan kode/huruf, munculkan `<MissingSlot />` (`border: 3px dashed #EA580C`, `borderRadius: 14px`) berisi tanda `?` yang berkedip.
Dynamic Flex Push with Inline Pill (`<DynamicFlexTextWithPill />`):
Baris teks di tengah layar (`display: 'flex'`, `alignItems: 'center'`, `gap: 16`).
Saat lencana kapsul (`border: 1px solid #22C55E`, `background: rgba(34,197,94,0.12)`) muncul di tengah/kanan kalimat, animasikan `maxWidth` dari `0px` ke `260px` dengan `spring()` sehingga kata-kata di sebelah kirinya terdorong bergeser ke kiri secara mulus.
Mixed Editorial Typography + Animated Highlight Strip (`<EditorialHeadline />`):
Kombinasikan Sans-Serif Medium (baris 1), Editorial Serif Bold Italic (`Playfair Display` / `Instrument Serif` pada baris 2), dan Extra-Bold Sans-Serif di atas pita sorotan (`scaleX: 0 -> 1`, `transformOrigin: 'left'`, `rotate: -1deg`) pada baris 3.
Wireframe Echo & Wave-Distorted Typography (`<WireframeEchoHeadline />` & `<WavyKineticWord />`):
Tambahkan 2–3 lapisan duplikat teks bergaris tepi tipis (`fill: 'none'`, `strokeWidth: 1`, `opacity: 0.25`) yang bergeser menyatu ke teks utama saat mendarat, atau gunakan `<feDisplacementMap>` + bintang 4-sudut (`✦`) untuk penekanan kata berenergi tinggi.
2. Kelompok Komponen Kartu UI, 3D Mockup, & Bento Dashboard
3D Isometric Device Pop-Out Rig (`<Device3DPopOutRig />`):
Tampilkan smartphone/PC dalam perspektif 3D (`perspective: 1200px`, `rotateX(12deg) rotateY(-18deg) rotateZ(14deg)`).
Saat fokus beralih ke data, luruskan rotasi perangkat ke `0deg` sambil dolly-in (`scale: 1 -> 1.45`) dan kaburkan perangkat (`blur(14px)`), sementara kartu utama melompat keluar (detach) dari layar perangkat ke tengah kanvas diikuti staggered cascade 3 kartu item di bawahnya (`gap: 14px`, opasitas menurun `1.0`, `0.75`, `0.45`).
Pinned Header Counter + Vertical Whip-Scroll Carousel (`<PinnedCounterCarousel />`):
Kunci Sticky Header Bar di bagian atas dengan angka total di kanan-atas yang berhitung mundur/naik secara real-time (`interpolate`).
Di bawahnya, gulirkan grup kartu item secara vertikal ke atas menggunakan `maskImage: 'linear-gradient(to bottom, transparent 0%, black 12%, black 85%, transparent 100%)'` dengan durasi `22 frame` (@30fps) per siklus scroll.
Synchronized Multi-Card Bento Dashboard (`<SynchronizedBentoDashboard />`):
Susun 4–5 kartu berbeda warna (Putih `#FFFFFF`, Oranye `#F04E23`, Hitam `#141416`, Hijau Lime `#B8E92E`, Ungu `#5238F2`) dalam satu layar CSS Grid.
Jalankan mikro-animasi di setiap kartu secara serempak: counter angka (`+201% -> +248%`), grafik garis kurva SVG, toggle switch bergeser aktif, cincin donut chart (`4% -> 99%`), batang equalizer memantul, playhead timeline menyapu titik diamond keyframe, dan kursor mengklik tombol `RENDER` $
ightarrow$ `DONE`.
2-Column Bento Form Camera Rig (`<BentoFormCameraRig />`):
Grid 2 kolom kartu input yang digerakkan naik secara kontinu (`translateY: +180px -> -140px`) seolah kamera melakukan vertical pan menuju tombol kapsul penuh di bawah. Kartu yang sedang aktif menyala dengan `border: 1.5px solid #22C55E` dan simulasi ketikan angka berkursor (`|`).
Perspective 3D Scrolling Card (`<Perspective3DMusicCard />`):
Kartu gelap bersudut membulat yang melayang miring di ruang 3D (`rotateX(14deg) rotateY(-18deg) rotateZ(6deg)`), di mana baris teks/item yang aktif tampil putih tajam (`blur(0px), opacity: 1, scale: 1.05`) sedangkan baris sebelum dan sesudahnya dibuat buram (`blur(3.5px), opacity: 0.35`).
3. Kelompok Komponen Taktil, Stiker Cutout, & Simulasi Interaktif
Halftone Cutout Sticker & Torn Paper Frame (`<HalftoneCutoutSticker />`):
Objek foto/ilustrasi (orang, bohlam, mesin tik, TV tabung, PC klasik, mikrofon, stopwatch) diberi filter monokrom/retro kontras tinggi dan dikelilingi garis tepi potongan kertas putih tebal (`drop-shadow` `#F4F1EA` berlapis `10px–14px` + bayangan jatuh `rgba(0,0,0,0.28)`).
Interactive Prompt-to-Canvas Preview (`<InteractivePromptCanvas />`):
Tampilkan kanvas pratinjau berbingkai hitam tebal di tengah layar dan gelembung chat prompt hitam di kanan-atasnya. Tepat pada frame saat gelembung prompt muncul, langsung ubah objek di dalam kanvas (misal: ukuran teks membesar `scale: 1 -> 1.85` dengan bouncy spring atau warna latar kotak berubah seketika).
Storyboard Grid with Magnifying Loupe (`<StoryboardGridWithLoupe />`):
Matriks kartu `6x3` berlabel waktu monospasi (`0.0s`, `2.5s`) yang dipindai oleh garis playhead merah-oranye dan objek kaca pembesar (`<MagnifyingLoupe />`) yang memperbesar isi kartu di dalam lingkaran lensanya (`scale: 1.35`).
Retro OS Warning Modal & Hand-Drawn Marker (`<RetroWarningModal />`):
Jendela pop-up retro ber-title bar dengan tombol `\[-] \[□] \[X]`, dipadukan dengan pita kata miring zig-zag (`<TiltedWordPills />`), animasi coretan lingkaran spidol merah (`strokeDashoffset`), dan tanda centang hijau (`✓`).
4. Kelompok Komponen Visualisasi Teknis, Hardware, & CTA Penutup
Arc Speedometer, Power Bar & Stamp Overlay (`<ArcGauge />` & `<StampOverlay />`):
Busur setengah lingkaran SVG dengan jarum berputar berbasis `spring()` (`-75deg` ke `+75deg`), bar konsumsi daya yang menghitung naik, serta stempel peringatan miring (`rotate(-8deg)`) yang menghantam layar dari `scale: 2.2` ke `1.0`.
Hardware Die, Audio Waveform, & Client-Server Flow (`<HardwareDieDiagram />` & `<AudioWaveformCloneComparison />`):
Penampang chip internal dengan blok komponen (`NPU`) yang menyala oranye terang saat kamera zoom-in; komparasi dua gelombang suara (waveform putih di atas vs merah-oranye di bawah); serta aliran titik paket data dari Server ke Laptop.
Horizontal Whip-Pan CTA with Cursor Click (`<HorizontalWhipCTAWithCursor />`):
Tampilkan teks singkat 2 kata di tengah layar, lalu banting kamera ke kanan secara cepat (`translateX: 0 -> -580px` dalam `10 frame` @30fps) sehingga sisa huruf terakhir masih terlihat sedikit di tepi kiri layar (`10–15%` partial edge framing) sementara tombol kapsul utama masuk ke tengah layar dan diklik oleh kursor tangan (`scale: 1 -> 0.93 -> 1.0`).
Orbital Identity Lockup & Comment Simulation (`<OrbitalIdentityLockup />` & `<CommentSimulationCTA />`):
Penutup berupa teks utama yang mendarat dengan per-character wave spring dikelilingi lintasan elips komet 3D (`zIndex` berganti antara `+10` di depan dan `-10` di belakang teks), atau simulasi kolom komentar yang mengetik otomatis (typewriter) beserta balasan admin.
---
BAGIAN V: STANDAR PRESISI WAKTU TRANSISI & FISIKA GERAKAN REMOTION
Berikut adalah rujukan hasil pengukuran frame-by-frame dari seluruh video referensi yang WAJIB digunakan AI saat menulis fungsi `interpolate()` dan `spring()` di Remotion:
Jenis Transisi / Gerakan	Durasi Presisi (@30fps / @60fps)	Mekanika Vektor & Kurva Easing di Remotion
1. Radial Iris Expansion	`5 Frame` (`0.167s`) / `10 Frame`	Lingkaran di pusat `(50%, 50%)` membesar dari `scale(0)` ke `scale(28)` dengan `Easing.bezier(0.7, 0, 0.15, 1)` hingga menutup `100%` layar.
2. 3D Device to UI Card Pop-Out	`11 Frame` (`0.367s`) / `22 Frame`	Perangkat 3D meluruskan rotasi ke `0deg`, `scale(1 -> 1.45)`, `blur(0 -> 14px)`, sementara kartu utama terlepas ke depan (`scale: 0.42 -> 1.0`) diikuti cascade 3 kartu anak (jeda `3f` per kartu).
3. UI Stack to Center Text Crossover	`9 Frame` (`0.300s`) / `18 Frame`	5f Exit: Kartu menyusut (`scale: 0.88`), naik (`dy = -5 px/f`), `blur(16px)`, `opacity(0)`. 1f Crossover. 4f Enter: Teks tengah naik (`Y: 317 -> 296px`) dan menajam (`blur: 10px -> 0px`).
4. Horizontal Whip-Pan (Overlapping)	`8–10 Frame` (`0.30s`) / `16–20 Frame`	Elemen lama terlempar ke kiri (`dx = -52 s/d -65 px/f`) dengan directional blur (`scaleX: 1.35`, `feGaussianBlur`). Tepat saat sisa elemen lama tinggal `10%` di tepi kiri, elemen baru sudah masuk dari tepi kanan.
5. Vertical Whip-Scroll Carousel	`22 Frame` (`0.733s`) / `44 Frame`	Grup kartu lama terdorong ke atas (`dy` puncak `-30 px/f`) melewati batas gradient mask atas sementara grup kartu baru naik dari bawah dengan `Easing.bezier(0.22, 1, 0.36, 1)`.
6. Paper Wash / Texture Cross-Fade	`6–9 Frame` (`0.25s`) / `12–18 Frame`	Pergantian warna kertas latar disertai lonjakan singkat `contrast(1.3)` dan keluar-masuknya stiker cutout dengan preset `bouncy` (`{ mass: 0.6, damping: 10, stiffness: 240 }`).
7. Staccato Beat / Flash Cut	`3–7 Frame` (`0.10–0.23s`) / `6–14 Frame`	Pemotongan cepat sinkron ketukan musik/suara atau 1-Frame White Flash (`#FFF8F3`) yang meluruh eksponensial selama `6–10 frame` saat memasuki scene 3D/klimaks.
8. Preset `spring()` Standar UI	`12–18 Frame` / `24–36 Frame`	`snappy`: `{ mass: 0.8, damping: 16, stiffness: 180 }` (Kartu/Teks/Modal).<br>`bouncy`: `{ mass: 0.6, damping: 10, stiffness: 240 }` (Stiker/Ikon/Stempel/Klik).<br>`smooth`: `{ mass: 1.0, damping: 24, stiffness: 120 }` (Kamera 2.5D/3D & Panning).
---
BAGIAN VI: ATURAN WAJIB VOICEOVER ELEVENLABS & SINKRONISASI AUDIO-VISUAL
AI wajib menggunakan ElevenLabs sebagai mesin pembuat suara (Text-to-Speech) dan mengikat seluruh timing pergantian scene, sorotan teks, hingga pemicu animasi objek ke timestamp kata yang dihasilkan oleh ElevenLabs.
Pre-Render Script dengan Endpoint `with-timestamps` (`scripts/generate-voice.ts`):
Panggil `POST https://api.elevenlabs.io/v1/text-to-speech/{voice\_id}/with-timestamps` menggunakan model `eleven\_multilingual\_v2` (atau `eleven\_turbo\_v2\_5`) dengan pengaturan `{ stability: 0.55, similarity\_boost: 0.80, style: 0.25, use\_speaker\_boost: true }`.
Simpan audio ke `public/audio/voiceover.mp3` dan konversi data `alignment` karakter menjadi array kata beserta `start`, `end`, `startFrame`, dan `endFrame` ke dalam `src/data/voice-timestamps.json`.
Durasi Komposisi Otomatis & Pemicu Visual Berbasis Kata (`Audio-Driven Triggers`):
Gunakan `calculateMetadata` di `Root.tsx` agar `durationInFrames = Math.ceil((audioDurationInSeconds + 1.5) \* fps)`.
Setiap kemunculan objek utama, pergeseran `<DynamicFlexTextWithPill />`, pembentangan `<HighlightStrip />`, putaran `<ArcGauge />`, hingga siklus scroll `<PinnedCounterCarousel />` wajib dipicu menggunakan `<Sequence from={word.startFrame}>` sesuai kata kunci yang diucapkan.
Setiap kata pada judul maupun subtitle menyala dari redup (`opacity: 0.25`) menjadi terang (`opacity: 1.0`) tepat saat `currentTime >= word.start`.
Pemasangan `<Audio />` & Background Music Ducking:
Pasang `<Audio src={staticFile('audio/voiceover.mp3')} volume={1.0} />` di root komposisi, dan terapkan audio ducking pada musik latar (`volume: 0.14` saat ada kata aktif yang diucapkan, dan naik ke `0.40` saat jeda transisi/outro).
