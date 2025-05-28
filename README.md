# Roman Urdu Emotion Detection & Response Generation 🤖💬

A comprehensive emotion detection system for Roman Urdu text that classifies emotions and generates appropriate responses using LLaMA 3.2 with Retrieval-Augmented Generation (RAG) and reinforcement learning optimization.

## 🎯 Project Overview

This system addresses the gap in Roman Urdu emotion analysis by implementing a local, offline solution that detects emotions (happy, sad, angry, neutral) and generates contextually appropriate responses with speech synthesis capabilities.

## ✨ Key Features

- **Roman Urdu Processing**: Specialized handling of Roman Urdu text and mixed-language usage
- **Multi-Model Emotion Detection**: Tested LLaMA 3.2:1B, Gamma:2B, and 3B parameter models
- **Retrieval-Augmented Generation (RAG)**: Context-aware response generation using vector stores
- **Speech Synthesis**: Audio response generation using StyleTTS2
- **Reinforcement Learning**: PPO-based optimization using user feedback
- **Local Deployment**: Completely offline operation without internet dependency

## 🛠️ Technology Stack

- **LLaMA 3.2:1B** - Core language model for emotion detection and response generation
- **FAISS** - Vector store for RAG implementation
- **sentence-transformers** - Text embeddings for similarity matching
- **StyleTTS2** - Text-to-speech synthesis for Roman Urdu
- **MongoDB** - Conversation history and feedback storage
- **Proximal Policy Optimization (PPO)** - Reinforcement learning framework



## 🚀 System Architecture

1. **Input Processing**: Roman Urdu text input
2. **Emotion Detection**: LLaMA model classifies emotion
3. **Context Retrieval**: RAG retrieves relevant past conversations
4. **Response Generation**: Generates appropriate Roman Urdu response
5. **Speech Synthesis**: Converts text to audio using StyleTTS2
6. **Feedback Loop**: User feedback for reinforcement learning
7. **Data Storage**: MongoDB for conversation tracking

## 📈 Key Results

- **Overall Accuracy**: 70.1% emotion detection
- **User Satisfaction**: Improved from 2.7 to 4.5 (out of 5) after reinforcement learning
- **Local Operation**: Complete offline functionality achieved
- **Response Quality**: Significant improvement through RAG integration

## 💻 Example Usage

```
Input: "Mujhe afsos hai."
Detected Emotion: Sad
Generated Response: "Mujhe bura laga sun ke aap udaas hain. Koi baat nahi, sab theek ho jayega!"
```

## 🗃️ Dataset

- **Training**: Roman-Urdu-English Code-Switched Emotion Dataset (Kaggle)
- **Testing**: Custom Roman Urdu sentences with emotion labels
- **Distribution**: Happy (27.4%), Sad (19.5%), Angry (22.8%), Neutral (30.3%)

## 🔧 Installation & Setup

```bash
# Clone repository
git clone https://github.com/manahilcpkhan/roman-urdu-emotion-detection.git
cd roman-urdu-emotion-detection

# Install dependencies
pip install -r requirements.txt

# Start MongoDB
mongod

# Run the system
python run.py (first run the model)
python app.py (to run the webpage)
```

## 🏆 Key Innovations

- **First Roman Urdu emotion detection system** with local deployment
- **RAG integration** for context-aware response generation
- **Reinforcement learning optimization** based on user feedback
- **Multi-modal output** with both text and speech responses
- **Offline operation** eliminating internet dependency

## 🔮 Future Enhancements

- Expand to formal Urdu and English support
- Add more nuanced emotion categories
- Improve speech synthesis quality for Roman Urdu
- Enhance model performance with larger datasets

---

*A novel approach to emotion detection in low-resource languages, demonstrating the effectiveness of modern NLP techniques for Roman Urdu processing.*