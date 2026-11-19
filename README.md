
## Hi, I'm Madhushri 👋

**Voice AI and ML engineer** in India.BE in AI Engineering, KLE Technological University, 2026. Open to full-time roles and research internships in speech, Indic NLP, LLM agents, or AI infrastructure.

Most of my work starts from a concrete failure mode in speech or agent systems—catching pronunciation errors that commercial ASR text smooths over, automating call audits that manual QA cannot scale, and logging telemetry so debugging is deterministic.

🌐 [Portfolio](https://madhushri-portfolio.pages.dev/) · 🎥 [Demo Video](PASTE_YOUR_LOOM_LINK_HERE) · 📧 [patilllmadhushri@gmail.com](mailto:patilllmadhushri@gmail.com)

---

### Problems & Solutions

#### Phoneme-Level Reading Assessment POC
- **The problem:** When building language-learning tools for children in Indic languages, commercial ASRs like Sarvam or Deepgram optimize for fluent transcription and language-model priors—smoothing over mispronunciations into "correct" text and hiding real reading errors.
- **The solution I built:** Built an audio-first reading assessment POC ([Demo Video](PASTE_YOUR_LOOM_LINK_HERE)) that evaluates phoneme-level pronunciation directly from raw speech using fine-tuned `wav2vec2`, Viterbi alignment, and Goodness of Pronunciation (`GOP`) scoring rather than relying on ASR text transcripts.

#### Automated Testing & Auditing System for Voice Agents
- **The problem:** Auditing voice agent calls manually by listening through hours of recordings is slow, error-prone, and difficult to scale across batches.
- **The solution I built:** Built a batch testing and auditing pipeline ([Portfolio](https://madhushri-portfolio.pages.dev/)) that analyzes call transcripts, flags potential conversational and flow issues, surfaces agent recommendations, and generates structured call- and batch-level reports to streamline debugging and QA.

#### Multilingual Indic Voice AI Agents (`Dialflo.ai`)
- **The problem:** Deploying conversational voice agents for Indic languages and real-world workflows requires reliable turn/state handling, ASR/TTS integration, and visibility into production call failures.
- **The solution I built:** Over 6 months as a Voice AI & Forward Deployed Intern at **Dialflo.ai**, built and deployed a production Kannada voice AI agent for the **ONEST project by EkStep Foundation** alongside English and Hindi agents—owning agent logic, ASR/TTS integration, testing, automation, deployment, transcript auditing, preprocessing, and prompt/pipeline improvements.

#### Agent Telemetry & Sandboxed Execution (`Quickcall.dev`)
- **The problem:** Debugging agent runs and executing candidate code across different environments breaks down without structured event logs and isolated, reproducible runtimes.
- **The solution I built:** During a 2-month AI Engineer internship at **Quickcall.dev**, built a telemetry pipeline capturing messages, tool calls, token usage, and errors as `JSONL` with `SQLite` (`WAL` mode) queuing and `PostgreSQL` sync, built a `Docker` sandbox harness for isolated execution, packaged cross-platform `Bun` executables (Linux, macOS, Windows), and contributed shared agent logic across a monorepo.

#### Autonomous Crop Disease Robot (IIT Bombay e-Yantra Finalist)
- **The problem:** Monitoring crop health across a farm-like arena requires combining real-time visual disease detection with reliable autonomous robot navigation.
- **The solution I built:** Trained a `YOLO` computer vision model to detect plant diseases from onboard camera images and integrated detection with autonomous field navigation.

---

### Current Focus

#### Closed-Loop ASR + TTS + CoT + GOP Pipeline *(In Progress)*
- **The problem I'm focusing on:** Combining speech recognition, speech synthesis, step-by-step reasoning, and phoneme-level pronunciation scoring (`GOP`) into a single closed loop—so a system can catch acoustic/pronunciation errors that text-only pipelines miss, reason over what to address next, speak targeted guidance back via `TTS`, and log turn-level metrics (`WER`, mispronunciation detection, latency, and reasoning traces).
