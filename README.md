# AI Learning Assistant

### Your 24/7 Study Buddy

Hey there! 👋 Ever find yourself stuck on a programming problem at 2 AM with no one to ask? We've been there too. That's why we built this AI Learning Assistant - your personal tutor that never sleeps.

## What This Does

Simply put: you give it learning materials (websites, PDFs, notes), and it becomes your personal expert on that topic. Ask any question and get instant, helpful answers.

**Real example from our testing:**
```
You: "I'm learning data structures. How do I rotate an array?"
Assistant: "Let me break this down. There are a few ways to rotate an array. The simplest is using a temporary array - here's the Python code..."
You: "Why would I use the reversal method instead?"
Assistant: "Great question! The reversal method is more space-efficient. Let me show you how it works..."
```

## Quick Setup (5 minutes tops)

### What You'll Need:
- Python (3.8 or newer)
- A free Google PaLM API key ([get one here](https://makersuite.google.com/app/apikey))

### Let's Get Started:

```bash
# 1. Download the project
git clone https://github.com/yourusername/ai-learning-assistant.git
cd ai-learning-assistant

# 2. Install what we need
pip install -r requirements.txt

# 3. Add your API key
echo "GOOGLE_PALM_API_KEY=your_key_here" > .env

# 4. Fire it up!
streamlit run src/ui/streamlit_app.py
```

That's it! Your browser should open with the assistant ready to help.

## How People Are Using This

### Computer Science Students
"Finally understand recursion! The assistant explained it with such simple examples that actually made sense."

### Bootcamp Learners
"When I got stuck on my capstone project at midnight, this thing saved me. It's like having a TA in your pocket."

### Self-Taught Programmers
"No more digging through Stack Overflow for hours. I just ask my question and get a clear explanation with code examples."

## What You Can Ask

Pretty much anything learning-related:

**Code Help:**
- "How do I implement binary search in Python?"
- "What's the difference between lists and tuples?"
- "Why is my sorting algorithm so slow?"

**Concept Explanations:**
- "Explain machine learning like I'm 10"
- "What exactly is time complexity?"
- "How do databases handle concurrent users?"

**Project Guidance:**
- "How should I structure my web app?"
- "Best practices for API design?"
- "Debugging tips for Python applications"

## Behind the Scenes

Here's the tech that makes it work:

- **Google's PaLM** - The brain that understands your questions
- **LangChain** - Organizes everything and finds the right answers
- **Streamlit** - The clean interface you interact with
- **Python** - Glues everything together

## For Developers

Want to tweak it or add features? Here's the structure:

```
ai-learning-assistant/
├── src/ui/              # The web interface
├── src/models/          # Talks to Google's AI
├── src/chains/          # The logic that processes questions
├── src/utils/           # Helper functions
└── data/               # Where learning materials live
```

To run tests:
```bash
pytest tests/
```

## We'd Love Your Help!

Found a bug? Have an idea to make it better? Here's how you can contribute:

1. Fork the repo
2. Create your feature branch
3. Make your changes
4. Send a pull request

Some areas we'd love help with:
- Adding support for more file types
- Making the interface even cleaner
- Improving how we handle different subjects
- Adding progress tracking

## License

This is open source under the MIT license. Use it, learn from it, build upon it!

## Shout Outs

Big thanks to:
- Google for the PaLM AI
- The LangChain team for making AI accessible
- Streamlit for the easy web framework
- All the students who tested this and gave feedback

---

**Ready to never get stuck learning again?** 

Clone the repo and give it a try. Your future self will thank you when you're cruising through that late-night study session!

*Built during the AI Demos Hackathon - Nov 2025*
