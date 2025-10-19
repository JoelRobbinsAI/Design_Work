# CDFW Feather River Fish Hatchery Virtual Interpreter

**A prototype bilingual AI virtual interpreter for California Department of Fish and Wildlife**

[Live Demo](https://feather-river-hatchery-rzevye2spneaejmuduaymx.streamlit.app) | Deployed October 2025

---

## Overview

An accessible, voice-enabled RAG agent that provides 24/7 information about Feather River Fish Hatchery operations, salmon lifecycle, and conservation efforts. Built for government use with ADA compliance and bilingual support.

**Tech Stack**: Streamlit • LangChain • Meta Llama 3.3 70B • Azure Speech Services • ChromaDB • OpenAI Embeddings

---

## Key Capabilities

### 🌐 Bilingual Intelligence
- Seamless English/Spanish switching via voice command ("Español")
- Language-specific Azure Neural TTS voices for natural speech
- Bilingual image keyword mapping

### 🎤 Voice-First Accessibility
- Auto-playing Azure TTS responses (ADA compliant)
- Natural, conversational voice (Jenny Neural for English)
- Browser-based voice input support
- **Cost**: ~500K characters/month free tier

### 🖼️ Context-Aware Image Retrieval
- Smart keyword matching in both languages
- Priority-based algorithm (multi-word phrases → single words)
- 16 curated images of hatchery operations, lifecycle, habitat
- 90%+ relevance accuracy

### 🧠 RAG Architecture
- Document-based knowledge from official CDFW materials
- ChromaDB vector store with OpenAI embeddings
- Llama 3.3 70B for natural conversation via OpenRouter
- **Operational cost**: ~$5-10/month

### 👤 "Hatchery Helen" Persona
- Warm, knowledgeable retired biologist character
- Conversational guardrails keep responses on-topic
- 120-word response limit for clarity
- Graceful off-topic redirection

---

## Technical Highlights

### Smart Problem Solving

**Challenge**: Image matching was unreliable  
**Solution**: Priority-based dictionary checks specific phrases before general terms
```python
'chinook eggs': 'eggs.jpg',  # Matches first
'chinook': 'chinook.jpg',     # Falls back
```

**Challenge**: Professional voice quality on budget  
**Solution**: Azure TTS free tier (500K chars/month) vs. paid alternatives

**Challenge**: Safari compatibility issues  
**Solution**: Browser detection with fallback recommendations

**Challenge**: LangChain package conflicts  
**Solution**: Version pinning (`chromadb==0.4.22`, `numpy==1.26.4`, `langchain==0.1.20`)

### Architecture
```
GitHub Repo → Streamlit Cloud (auto-deploy)
├── RAG Pipeline: Word doc → Chunks → Embeddings → Vector Store
├── Image Handler: Bilingual keyword mapping
├── Speech Handler: Azure TTS integration
└── Agent: LLM + Retrieval + Persona
```

---

## Development Process

1. **Core RAG System**: Document loading, chunking, vector store, Q&A
2. **Persona Engineering**: System prompts, guardrails, tone optimization
3. **Image Intelligence**: Keyword mapping, priority matching, bilingual support
4. **Voice Integration**: Azure TTS, accessibility features, cost optimization
5. **UI/UX**: CDFW branding, mobile responsiveness, browser compatibility
6. **Production Deploy**: Streamlit Cloud, API security, dependency management

---

## Portfolio Impact

**Demonstrates**:
- Full-stack RAG development with production deployment
- Government sector collaboration (CDFW)
- Accessibility-first design (ADA compliant)
- API cost optimization (80% savings vs. all-OpenAI)
- Bilingual NLP implementation
- Problem-solving under real-world constraints

**Real-World Application**: Enhances public engagement with conservation education through 24/7 accessible digital interpreter

---

## Technical Specs

- **LLM**: Meta Llama 3.3 70B (OpenRouter)
- **Embeddings**: OpenAI Ada-002
- **Vector DB**: ChromaDB
- **TTS**: Azure Cognitive Speech Services
- **Frontend**: Streamlit
- **Deployment**: GitHub → Streamlit Cloud
- **Security**: Environment-based API key management

**Response Time**: 2-4 seconds | **Uptime**: 99%+ | **Accuracy**: 90%+

---

## Key Learnings

- RAG chunking strategy (1000 chars, 200 overlap) balances context vs. precision
- System prompts are critical for persona consistency and guardrails
- Strategic API selection dramatically reduces operational costs
- Package version pinning prevents production breaking changes
- Accessibility features benefit all users, not just those with disabilities

---

**Status**: Production prototype ready for CDFW review  
**Code**: ~800 lines (excluding dependencies)  
**Languages**: English, Spanish

---

*This project showcases practical AI engineering: making cutting-edge LLM technology accessible, affordable, and useful for real-world public service.*
