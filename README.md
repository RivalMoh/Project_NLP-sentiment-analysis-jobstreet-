# 🎯 JobStreet App Sentiment Analysis - My First NLP Adventure!

<div align="center">

![NLP](https://img.shields.io/badge/NLP-Sentiment%20Analysis-blue)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-RNN%7CLSTM%7CGRU-green)
![Accuracy](https://img.shields.io/badge/Accuracy-95%25-brightgreen)
![Language](https://img.shields.io/badge/Language-Indonesian-red)

*🚀 Exploring the world of Natural Language Processing through real-world data!*

</div>

## 🌟 What's This All About?

Welcome to my **first-ever NLP project**! 🎉 

Ever wondered what people *really* think about JobStreet app? I did too! So I built this sentiment analysis system that can read through thousands of Google Play Store reviews and tell us whether users are happy 😊, frustrated 😠, or just meh 😐 about the app.

This project is my journey into the fascinating world of **Natural Language Processing**, where I learned to teach computers how to understand human emotions hidden in text!

**👨‍💻 Created by:** Rival Moh. Wahyudi  
**📧 Email:** vallllwhy@students.unnes.ac.id  
**📍 Location:** Semarang, Indonesia  
**🎓 Status:** First NLP Project - Learning & Growing!  

## 🗂️ Project Adventure Map

Here's what you'll find in my NLP playground:

```
2_NLP_Sentiment_(Jobstreet)/
├── 📊 Scraping.ipynb                                    # 🕷️ My web scraping adventure!
├── 🧠 Project Sentiment Analysis_Rival Moh. Wahyudi.ipynb  # 🎯 Where the magic happens!
├── 📝 jobstreet_review.csv                              # 📦 Raw treasure from Google Play
├── ⚡ checkpoint.csv                                     # 🔄 Halfway checkpoint (smart move!)
├── ✨ final.csv                                         # 🏆 The final masterpiece
├── 📋 requirements.txt                                   # 🛠️ All the tools I needed
├── 📚 combined_root_words.txt                           # 🌱 Indonesian word roots
├── 💬 combined_slang_words.txt                          # 😎 Cool slang translator
├── 🚫 combined_stop_words.txt                           # ⛔ Words to ignore
├── 🎭 sentimentword.txt                                 # 💝 Emotion detector dictionary
└── 📖 README.md                                         # 📍 You are here!
```

## 🚀 What Makes This Project Special?

As my **first dive into NLP**, I'm pretty excited about what I built! Here's what my system can do:

### 🎪 **The Show-Stoppers:**
- **🕸️ Smart Web Scraping**: Automatically grabs 20,000+ real user reviews from Google Play Store
- **🧹 Indonesian Text Wizard**: Handles messy Indonesian text like a pro (slang, typos, emojis - you name it!)
- **🎭 Emotion Detective**: Classifies sentiments into Positive, Negative, and Neutral with 95% accuracy!
- **🤖 Triple AI Power**: Built 3 different neural networks (RNN, LSTM, GRU) and compared them
- **📊 Smart Feature Engineering**: Uses TF-IDF to turn text into numbers that machines understand

### 🎯 **Why This Matters:**
- **Real-world data**: Not just toy datasets - actual user opinions!
- **Indonesian language focus**: Tackled the challenges of processing Bahasa Indonesia
- **End-to-end pipeline**: From raw data to deployed model
- **Performance comparison**: Learned which model works best for what

## 🛠️ Getting Started (Let's Build This Together!)

### Step 1: Set Up Your Environment
```bash
# Clone or download this repo first!
pip install -r requirements.txt
```

### Step 2: Get NLTK Ready (One-time setup)
```python
import nltk
nltk.download('punkt')      # For tokenization
nltk.download('stopwords')  # For removing common words
```

### Step 3: Ready to Rock! 🎸

## 🎬 The Journey: From Zero to NLP Hero!

### 🕷️ **Phase 1: The Great Data Hunt** (`Scraping.ipynb`)
*Where I learned that data doesn't just appear magically!*

My first challenge was getting real data. I discovered the amazing world of web scraping:
- 🎯 **Mission**: Collect 20,000 authentic JobStreet app reviews
- 🌏 **Target**: Indonesian users on Google Play Store  
- 🏆 **Result**: A treasure trove of real user opinions!

**What I learned:** Data collection is harder than I thought, but super rewarding when you see real data flowing in!

### 🧠 **Phase 2: The Text Transformation Magic** (`Project Sentiment Analysis_Rival Moh. Wahyudi.ipynb`)
*This is where I became a text wizard! ✨*

#### 🧹 **The Cleaning Adventure:**
Indonesian text is WILD! Here's how I tamed it:

1. **😀 Emoji Detective Work**: 
   - Turned `:)` into "senang" (happy)
   - Converted 😊 into readable Indonesian emotions

2. **🔧 Text Surgery**:
   - Removed messy stuff: @mentions, #hashtags, URLs, numbers
   - Fixed weird spacing and punctuation chaos

3. **💬 Slang Translator**: 
   - "gak" → "tidak" (no)
   - "bgt" → "banget" (very)
   - "lu" → "kamu" (you)
   - *Handled 500+ Indonesian slang words!*

4. **🌱 Word Root Finder**:
   - "berlari" → "lari" (running → run)
   - Used Sastrawi stemmer for Indonesian

5. **🎯 Smart Word Filtering**:
   - Removed common words that don't add meaning
   - Kept the juicy, emotional words!

#### 🎭 **The Emotion Scoring System:**
I built a sentiment calculator that reads Indonesian emotions:
- **Positive words** get positive points ➕
- **Negative words** get negative points ➖  
- **Final score** determines: Happy 😊 | Sad 😢 | Neutral 😐

#### 🤖 **The AI Battle Royale:**
I trained THREE different neural networks and made them compete!

**🥇 Team Simple RNN:**
- *The Speedy Gonzales* - Fastest training (2 seconds per epoch!)
- 128 neurons working hard
- Great for beginners (like me!)

**🥈 Team LSTM:**
- *The Memory Master* - Never forgets important parts of text
- Best at understanding context
- My personal favorite for complex sentences

**🥉 Team GRU:**
- *The Balanced Fighter* - Good speed + good memory
- Sweet spot between RNN and LSTM
- Perfect compromise!

## 🏆 The Epic Results!

*Plot twist: All my models performed like absolute champions!* 

All three neural networks achieved **95% accuracy** 🎯 - I couldn't believe it when I first saw these numbers!

- **🚀 Simple RNN**: *The Speed Demon* (~2 seconds per epoch) - Perfect for quick experiments!
- **🧠 LSTM**: *The Context King* - Amazing at remembering important details across long reviews
- **⚡ GRU**: *The Sweet Spot* - Best balance of speed and memory

**My biggest surprise:** Even the "simple" RNN performed just as well as the complex ones! Sometimes simple solutions work best.

## 🛠️ The Tech Arsenal (What I Used)

**Data Collection & Scraping:**
- `google-play-scraper` - My gateway to real user reviews
- `pandas` & `numpy` - Data manipulation superheroes

**Indonesian Text Processing:**
- `nltk` - Natural language toolkit (my NLP Swiss Army knife!)
- `Sastrawi` - Indonesian language stemmer (absolute lifesaver!)
- `fuzzywuzzy` - Fuzzy string matching for typo correction
- `emoji` - Emoji to text converter

**Machine Learning Magic:**
- `tensorflow/keras` - Deep learning framework (where the AI lives!)
- `scikit-learn` - ML utilities and TF-IDF vectorizer

**The Process Flow:**
```mermaid
🌐 Google Play Reviews → 🧹 Text Cleaning → 🔤 Tokenization → 
📊 TF-IDF Features → 🤖 Neural Networks → 😊😐😢 Sentiment Labels
```

## 📚 What's Inside Each File?

- **`jobstreet_review.csv`** 📦: *The gold mine* - 20,000 raw reviews straight from Google Play
- **`checkpoint.csv`** ⚡: *My safety net* - Preprocessed data saved at the halfway point (learned this the hard way!)
- **`final.csv`** ✨: *The masterpiece* - Clean data with sentiment labels ready for modeling
- **`sentimentword.txt`** 🎭: *The emotion decoder* - Indonesian sentiment lexicon I used for scoring
- **Text dictionaries** 📚: *My Indonesian language helpers* - Custom dictionaries for slang, stop words, and root words

## 🚀 My Learning Journey & Challenges

### 🤯 **Biggest "Aha!" Moments:**
1. **Data is messy!** Real-world text has SO much noise - emojis, typos, slang, abbreviations
2. **Indonesian is complex** - Handling "aku", "gue", "saya" (all mean "I") was tricky
3. **Simple can be powerful** - My basic RNN performed just as well as fancy LSTM!
4. **Feature engineering matters** - TF-IDF was crucial for turning text into numbers

### 😅 **Challenges I Overcame:**
- **Slang dictionary creation** - Had to manually map hundreds of Indonesian slang words
- **Memory management** - 20,000 reviews crashed my laptop a few times!
- **Model comparison** - Learning to properly evaluate and compare different architectures
- **Text preprocessing pipeline** - Getting the order of operations right took several attempts

## 🔮 What's Next? (Future Adventures)

I'm just getting started! Here's what I want to explore next:

- **🤖 Transformer models**: BERT, IndoBERT - the next level of NLP!
- **📊 Interactive dashboard**: Build a web app where people can analyze their own text
- **🎯 Aspect-based analysis**: Not just positive/negative, but WHY they feel that way
- **📱 Real-time analysis**: Live sentiment tracking of app reviews
- **🌏 Multi-language support**: Expand beyond Indonesian

## 💭 My Reflection

Building this as my first NLP project was both challenging and incredibly rewarding! I learned that:

- **Real data is messy** but way more interesting than clean datasets
- **Indonesian NLP** has unique challenges that made this project special
- **Deep learning isn't magic** - it takes careful data preparation and experimentation
- **Documentation matters** - Writing this README helped me understand my own journey better!

## 📬 Let's Connect!

I'd love to hear from fellow NLP enthusiasts, especially beginners like me! 

- **📧 Email**: vallllwhy@students.unnes.ac.id
- **📍 Location**: Semarang, Indonesia
- **💬 Status**: Always learning, always curious!

*Feel free to reach out if you want to discuss NLP, share experiences, or just say hi!* 👋

---

<div align="center">

**⭐ If this project helped or inspired you, please give it a star! ⭐**

*Made with ❤️ and lots of ☕ by a curious NLP beginner*

</div>