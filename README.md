# AI-Powered Video Vocabulary Extraction Pipeline
Team Members: Yuqian Wang, Patrick Zhu, Xinping Xue

## Project Title & Description
Title: Intelligent Video Analytics Platform - Vocabulary Extraction & Analytics Pipeline
Description: A production-grade data engineering pipeline that ingests video content, extracts fine-grained units (vocabulary, phrases) through multi-modal AI processing, and stores structured learning data for downstream analytics. The pipeline demonstrates end-to-end data engineering principles including event-driven architecture, multi-stage data transformation, distributed storage, and observability.

## Preliminary Data Sources
1. Video Files (Multiple formats: MP4, MOV, etc.)
- User-uploaded videos via GCS
- Sample datasets: Khan Academy clips, lecture recordings, videos on internet
2. Speech-to-Text Data (WhisperX API via Replicate)
- Real-time ASR results with word-level timestamps
- API: https://replicate.com/victor-upmeet/whisperx
- Output: Structured JSON with segments, confidence scores, speaker diarization
3. Multi-modal AI Analysis (Google Cloud Vertex AI - Gemini)
- Video understanding + transcript analysis
- Vocabulary annotations with evidence spans
- API: Vertex AI Gemini 2.0 models
4. Vocabulary Database
- Pre-existing vocabulary units
- External dictionary APIs (potential integration with WordNet, Oxford API)



