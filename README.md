# 🏥 Telehealth Note Automation


<img width="1781" height="356" alt="image" src="https://github.com/user-attachments/assets/30edc3a8-5303-4f03-b43e-4afb60f865f6" />


Automatically transcribe therapy sessions and generate structured clinical progress notes — hands-free.

What This Does

A fully automated pipeline that takes a therapist's phone call recording and turns it into a structured progress note — with zero manual effort beyond a single tap.

**One tap. That's it.**

🔄 How It Works

```
📱 iPhone Call Recording
        ↓
📁 Drop into OneDrive (Incoming folder)
        ↓
⚙️  Make.com detects new file instantly
        ↓
🎙️  Whisper AI transcribes audio
        (Arabic, English, or mixed — no setup needed)
        ↓
🤖  GPT generates structured progress note
        ↓
📂  Files saved to client folder automatically
        ├── transcript_2026-05-01_1037.txt
        └── ai_results.docx  ← all notes in one document
```

---

## 🗂️ Output Structure

```
📁 Outgoing/
    📁 Anna Karenina/
        📄 transcript_2026-05-01_1037.txt
        📄 transcript_2026-05-02_0945.txt
        📄 ai_results.docx   ← all session notes, appended
```

Each note in `ai_results.docx` is labeled with its transcript reference so the clinician can always trace back to the source.

---

## ⚙️ Setup

### Prerequisites
- Make.com account (Core plan or higher)
- OpenAI API key with credits
- Microsoft OneDrive account

### OneDrive Folder Structure
Create two folders in your OneDrive:
- `Incoming` — drop recordings here
- `Outgoing` — processed files appear here automatically

### File Naming Convention
Name your recording files using this format:
```
[session_type]_[Client Name].m4a
```

**Examples:**
```
client_Anna Karenina.m4a
parent_John Smith.m4a
support worker_Emma Davis.m4a
```


## 📋 Customising the Progress Note

The AI prompt can be updated inside Make.com to match your preferred note format — whether that's DAP, SOAP, or a custom structure.

---


## 👩‍💻 Built by

**Inesa Poghosyan** — Python backend engineer & API integration specialist  
[Upwork Profile](https://www.upwork.com/freelancers/~01cb4fcd377b79af10?mp_source=share)
