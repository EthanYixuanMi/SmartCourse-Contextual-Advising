# Smartcourse Contextual Advising

[![arXiv](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/xxxx.xxxxx)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](#)
[![License](https://img.shields.io/badge/License-MIT-green)](#license)

## 🔍 Overview

SmartCourse is a university course management and AI-driven advising system that provides personalized course recommendations based on a student's transcript and degree plan. This repository is an enhanced version of our original course project, extended for research and evaluation purposes.

> This project is based on the original coursework project:  
> [CS-Course-Project-in-Wenzhou-Kean-University/CPS3320](https://github.com/EthanYixuanMi/CS-Course-Project-in-Wenzhou-Kean-University/tree/main/CPS3320)


## ✨ New in This Version

This research version expands the original project with:
- 📊 Experimental evaluation on 25 advising queries
- 🎯 Novel contextual prompts integrating transcripts and four-year plans
- 🧠 Local LLM (via Ollama) for context-aware recommendations
- 📐 Custom metrics: `PlanScore`, `PersonalScore`, `Lift`, and `Recall`
- 🧪 Context ablation experiments comparing 4 modes (full, no transcript, no plan, question-only)


## 🧠 How It Works

SmartCourse supports three user roles:
- **Student**: Enroll/drop courses, view grades, and request AI suggestions
- **Instructor**: Assign grades and review student enrollment
- **Administrator**: Manage course catalog and switch LLM models


All interactions can happen through:
- ✅ Command-Line Interface (CLI)
- 🌐 Gradio-based GUI


The AI Advising Module uses structured prompts that combine:
[Transcript]()
[Degree Plan]()
[Student Question]()
to provide personalized suggestions via a local LLM (e.g., LLaMA3.1:8B through Ollama).

## 🛠 Installation

### 🔧 Requirements
- Python 3.8+
- Gradio, Requests

```bash
pip install gradio requests
```


## 🗂️ Required Files
- course_list.txt
- account.txt (auto-created)
- enrolled_courses.txt
- cps_plan.txt (sample four-year plan)


## ▶️ Running the App
CLI:
```bash
python main.py
```

GUI (Gradio):
```bash
python ui_gradio.py
```


## AI Integration (via Ollama)
1. Install [Ollama](https://ollama.com/download)

2. 







