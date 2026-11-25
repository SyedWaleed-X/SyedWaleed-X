<h1 align="center">Syed Waleed</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2600&pause=900&color=E8E2D6&center=true&vCenter=true&width=640&lines=AI+engineer;GPU+video+pipelines+that+render+at+240+fps;RAG+systems+over+thousands+of+documents;Tools+that+agents+and+people+drive+together;Learning+IoT+%2B+robotics" alt="AI engineer · GPU video pipelines · RAG systems · agent tooling · learning IoT and robotics">
</p>

<p align="center">
I build systems where performance is the feature: AI passes that run once and are cached,
GPU pipelines measured frame by frame, and interfaces that an AI agent and a person can use
through the same functions. Now also learning IoT and robotics, where the same habits
(measure first, bounded resources, real-time loops) carry over to hardware.
</p>

---

### KinetixHTML: a video editor where an edit is code

<a href="https://github.com/SyedWaleed-X/kinetix-html">
  <img src="media/burn.webp" width="100%" alt="LET THE WORLD BURN, an anime edit made with KinetixHTML: the sung words LET IT ALL BURN land on their beats, the Colossal Titan burns, and a figure turns to ash">
</a>

<p align="center"><sub><b>LET THE WORLD BURN</b>, 6 s of a 45 s edit. Fan edit of <i>Attack on Titan</i> and
<i>Mushoku Tensei</i> for demonstration; the anime belongs to its owners.</sub></p>

Every edit is an `edit.html` (HTML, CSS, JS, GLSL) rendered frame-exact on the GPU and
encoded in the browser with WebCodecs; only the 1-second segments whose draw commands changed
re-render. Rotoscoping (SAM 2.1 + MatAnyone2), depth and optical flow are cached AI passes.
One typed Python capability registry generates both the CLI and an MCP server, so an agent
cuts, looks at frames, patches and exports through the same functions a person uses in the
Studio. The edit above was made with it.

| Measured on one RTX 3060 | |
|---|---|
| 60 s 1080p30 composition, full render | **12.8-13.6 s** (HyperFrames 0.9.9: 122.4 s · Remotion 4.0.540: 244.3 s) |
| Change one value, re-export | **2 of 48 segments, 2.3 s** (rivals re-render everything) |
| 47 s 1080p60 anime edit with 69 cuts, 6 shader transitions, 9 type styles | **142 fps** full render |
| Test suite | **295** tests with real browser + GPU checks |

**[→ kinetix-html](https://github.com/SyedWaleed-X/kinetix-html)**

---

### Other work

**[ai-keystone-project](https://github.com/SyedWaleed-X/ai-keystone-project)**: a RAG-powered
corporate API. A REST service (FastAPI, PostgreSQL, Docker) with CRUD over company data and a
question-answering endpoint that does semantic search over a document library (txt, pdf) and
hands only the relevant passages to Gemini, so answers come from private data the model was
never trained on, however many documents there are.

**[dealersflow-fyp](https://github.com/SyedWaleed-X/dealersflow-fyp)**: my final year project
(in progress).

---

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,js,html,css,fastapi,postgres,docker,pytorch,git,linux&perline=10" alt="Python, JavaScript, HTML, CSS, FastAPI, PostgreSQL, Docker, PyTorch, Git, Linux">
</p>
<p align="center"><sub>WebGL2 / GLSL · WebCodecs · FFmpeg · MCP · RAG · learning IoT + robotics</sub></p>
