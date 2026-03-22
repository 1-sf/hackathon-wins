# 👋 Akhil Dhavala

Ads at Google, based in the Bay Area.

4+ years building large-scale ads systems — ranking pipelines, pCTR feature analysis, pre-ranking debugging, auction-stage optimization, and experimentation frameworks across Search, AI Overviews, and AI Mode. I combine strong systems engineering with ML intuition and a data analysis mindset to ship things that move metrics.

Outside of work I compete in ML hackathons, explore applied AI ideas, and build quick end-to-end prototypes.

📎 [LinkedIn](https://linkedin.com/in/1sf)

---

## 🔧 Skills

**Ads & ML**
`pCTR modeling` `pre-ranking` `auction systems (eCPM, quality score)` `ranking pipelines` `rejection funnel analysis` `ad-format optimization` `counterfactual analysis` `ablation studies`

**Experimentation & Data**
`A/B testing` `funnel metrics` `experiment dashboards` `behavioral data analysis` `feature analysis`

**Languages & Infra**
`Python` `Go` `C++` `SQL` `gRPC` `distributed systems` `low-latency pipelines`

**ML / AI (Hackathons & Projects)**
`TensorFlow` `EfficientDet` `BERT` `RAG pipelines` `vector search` `embeddings` `LLM pipelines` `voice synthesis` `prompt engineering`

---

## 🏆 Hackathon Wins

### 🥇 1. Verkada Hackathon — 1st Place

**Project: Golden Eye** — Real-time object monitoring across multi-camera CCTV

- Fine-tuned [EfficientDet](https://arxiv.org/abs/1911.09070) on ~500 labeled frames extracted from HLS streams across 5 cameras
- Built inference pipeline that triggers real-time alerts when a tracked object disappears from the scene
- Delivered a fully working live demo — won first prize

---

### 🥇 2. TEDAI Multimodal Hackathon — Grand Prize

**Project: NeuroLearn** — AI-powered adaptive learning using brain-wave signals

- Used brain-wave data (Neurosity headset + SDK) to gauge student focus in real time and dynamically surface relevant lecture snippets
- When engagement dropped, a voice model (ElevenLabs) narrated the content through a personalized "role-model" persona
- Built a knowledge graph over time to recommend new content based on individual interest and learning history
- Won the top prize under tight hackathon constraints
- [Devpost](https://devpost.com/software/neurolearn-son69a)

---

### 🥈 3. SF AI Hackathon (MongoDB + AI partners) — 2nd Place

**Project: Junto** — Real-time AI debate between two characters grounded in live news

- Indexed latest news articles using BERT 80M 32K embeddings (TogetherAI serverless endpoints) stored in MongoDB Atlas vector search
- Built a RAG pipeline that retrieves relevant document chunks per debate turn — accounting for both the topic and the opposing speaker's prior comments — then sends to Claude (Anthropic) to generate each speaker's response
- Fine-tuned character voices in ElevenLabs for audio output; streamed responses in real time
- Overcame latency and response-quality challenges to produce a clean demo-ready prototype
- [Devpost](https://devpost.com/software/junto-c8bute)

---

### 🥉 4. RunPod Hackathon — 3rd Place

**Project: Brain-signal action classification** — Structured EEG data → intent classification

- Input: 8×8 covariance matrices from Neurosity headset (covariances across 8 sensors), 400K+ records
- Evaluated BERT and convolution-based models; found non-linear discriminative models (Random Forest) outperformed sequence models on structured tabular EEG data
- Achieved **81.2% test accuracy**; saved model, containerized with Docker, deployed on RunPod serverless
- [GitHub](https://github.com/one-shot-finish/runpod_hack) · [X post](https://x.com/one_shot_finish/status/1792757800441151762)
