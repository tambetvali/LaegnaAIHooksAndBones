![Architecture diagram](../../Rooted/Images1/LaegnaAI_Architecture_1.jpg)

<br>

# Chapter 0 — The Three Steps of Growing AI Capability

In each step, the AI access interface is updated:
- Using the *initial guide*, you can **access** an AI or **install it yourself**.
- Using the *later parts*, it might ***need*** a *tech-savy individual* or *professional service* for you,
  - but **none of** them needs *special science*: mostly, ***installation*** of ***application*** as usual,
  - or **installation** of application *using terminal* - often it's just ***copy-pasting*** one line and ***pressing enter***.

---

Modern AI capability grows in layers. Most people, families, communities, and organizations follow a natural progression:

1. **Basic AI functionality**  
2. **Document collections and context**  
3. **Training and fine‑tuning**

This chapter introduces these steps in a simple, practical way. It is written for everyday users, for those who guide them, and for anyone researching how people adopt AI tools.

---

## 1. Basic AI Functionality

The first step is simply *getting access to an AI assistant* and learning how to use it effectively. This can be done through online services or local tools.

### 1.1 Connecting to Online AI Services (CoPilot, ChatGPT)

Most users begin with cloud‑based AI systems. These services offer:

- Natural language chat  
- Writing and editing assistance  
- Coding help  
- Document summarization  
- Image generation  
- Access to plugins, extensions, and integrations  

Creating an account is simple: sign up, verify email, and optionally subscribe for higher‑tier models. These systems require no installation and are ideal for beginners.

### 1.2 Installing Local AI Tools

Local AI tools run models directly on your computer. They vary in complexity and capability:

| Tool | Difficulty | What It Offers |
|------|------------|----------------|
| **Jan** | Easy | One‑click installation, built‑in chat, simple model downloads |
| **GPT4All** | Intermediate | Local models, document reading, plugins, external client connections |
| **Ollama** | Intermediate | Simple command‑line tool, fast model downloads, local API server |
| **LM Studio** | Advanced | Model management, server mode, API endpoints, integration with external apps |

#### Jan (easy)
- Install the app  
- Download a small model  
- Start chatting  
- Minimal configuration  

#### GPT4All (intermediate)
- Install the desktop app  
- Choose from many free models  
- Load documents for contextual chat  
- Connect external clients (VSCode, browser extensions)  
- Run a local API endpoint for other apps  

#### Ollama (intermediate)
- Install via a simple installer  
- Run models with a single command (`ollama run llama3`)  
- Pull models from a large community library  
- Expose a **local API** that many tools can connect to  
- Works well with VSCode, Obsidian, LogSeq, and custom scripts  

#### LM Studio (advanced)
- Install the application  
- Download or import models (GGUF and others)  
- Run a local API server  
- Integrate with external tools (VSCode, LogSeq, custom apps)  
- Manage multiple models and advanced settings  

This step teaches users how to combine built‑in chat with external clients and services.  
Beginners may stay with Jan or online AI.  
Intermediate users often adopt GPT4All or Ollama.  
Advanced users build full ecosystems around LM Studio.

---

## 2. Document Collections and Context

Once basic AI usage is comfortable, the next step is giving the AI *context*—your documents, notes, archives, and knowledge bases.

### 2.1 Local AI Tools for Document Reading

Tools like **GPT4All**, **Ollama (via plugins)**, and **LM Studio** can ingest:

- PDFs  
- Markdown files  
- Text archives  
- Knowledge bases  
- Research papers  

This allows the AI to answer questions using your own material.

### 2.2 Knowledge Management Tools

To organize and maintain document collections, users can choose:

| Tool | Difficulty | Capabilities |
|------|------------|--------------|
| **LogSeq** | Easy | Local graph notes, backlinks, plugins, simple AI integrations |
| **VSCode** | Intermediate / Advanced | Extensions for AI chat, code assistance, documentation workflows |

#### LogSeq (easy)
- Install the app  
- Create a graph  
- Add notes, PDFs, and pages  
- Use AI plugins for summarization and Q&A  
- Connect to GPT4All, Ollama, or LM Studio through community extensions  

#### VSCode (intermediate/advanced)
- Install AI extensions (free or paid)  
- Connect to local or cloud models  
- Use AI to refactor code, generate documentation, or analyze files  
- Integrate with **Ollama**, **GPT4All**, or **LM Studio** via local API endpoints  

This step transforms AI from a general assistant into a personalized knowledge worker.

---

## 3. Training and Fine‑Tuning

The final step is the most powerful: *teaching the AI new skills* or adapting it to your environment.

### 3.1 Tools for Training

Users can approach this at different levels:

| Tool | Difficulty | Purpose |
|------|------------|---------|
| **LitGPT** | Easy | Simple fine‑tuning workflows, guided setup |
| **Python‑based bots (pip)** | Intermediate | Specialized models (tiny, small, medium, large), experimental or domain‑specific |
| **PyTorch** | Hard | Full control over training GPT‑style models |

#### LitGPT (easy)
- Install with a few commands  
- Load a small model  
- Fine‑tune on your own text  
- Ideal for beginners with guidance from a tech‑savvy friend  

#### Python bots (intermediate)
- Install via pip  
- Explore fine‑tuning options  
- Work with experimental or specialized models  
- Learn how models behave with different datasets  

#### PyTorch (hard)
- Build or modify GPT architectures  
- Train on custom datasets  
- Convert models to formats used by ChatGPT, CoPilot, or community AIs  

### 3.2 How Users Access Training

Most end users don’t start alone—they get help:

- A tech‑savvy friend installs LitGPT  
- A professional sets up a training environment  
- A community shares models and scripts  
- A company provides curated datasets  

Training becomes a continuous process: start small, adjust, expand.

### 3.3 Organizational Training and Administration

Larger groups—families, villages, companies, corporations, governments—often have administrators who:

- Collect and organize documentation  
- Label data  
- Convert files into formats suitable for different models  
- Maintain consistency across tools and environments  

Different models require different approaches:

- **Small models** are sensitive:  
  - Confusing phrasing or unrelated content can cause hallucinations  
  - Even warning labels may disrupt expected outputs  

- **Large models** are robust:  
  - They can handle mixed, unlabelled, or contradictory data  
  - They learn patterns positively, negatively, or relationally  
  - They stabilize through volume and diversity  

This mirrors human learning: some people get confused by unclear information, others clarify it, and some discover hidden patterns and transform them into insight.

---

## Why This Matters for Users and Market Researchers

This three‑step progression reflects how real people adopt AI:

- **Simple users** start with online AI or Jan.  
- **Growing users** adopt GPT4All, Ollama, or LM Studio.  
- **Power users** begin training and fine‑tuning.  
- **Organizations** build structured AI ecosystems.  

Understanding this progression helps:

- Educators guide learners  
- Developers design tools  
- Communities build shared AI resources  
- Market researchers identify needs and gaps  
- Administrators plan long‑term AI strategies  

This chapter sets the foundation for everything that follows.

# Setting up Ollama and Open WebUI in a way a non‑technical user can understand and operate

## What Ollama is in practical terms
Ollama is a small program that runs AI models on a computer. It handles:

- downloading a model  
- keeping it ready  
- answering questions when another program asks  

A non‑technical user does not need to know how it works internally. They only need to know:

- it must be installed once  
- it must stay running in the background  
- it provides the “engine” that other tools use  

A technical friend or family member can install it by following the official instructions for Windows, macOS, or Linux. These instructions are written step‑by‑step and do not require guessing.

---

## What Open WebUI is in practical terms
Open WebUI is a website that runs on the user’s own computer. It provides:

- a chat window  
- buttons for settings  
- a list of available models  
- a place to type questions  

It connects to Ollama automatically once configured.  
The non‑technical user only needs to:

- open a browser  
- go to the local address (usually shown after installation)  
- start chatting  

Everything else is handled by the person who sets it up.

---

## What a non‑technical user needs to ask for
A non‑technical user only needs to know how to ask for help in simple terms. Typical requests:

- “Please install Ollama so I can run local AI models.”  
- “Please set up Open WebUI so I can use it in my browser.”  
- “Please add the model I want to use.”  
- “Please make sure it starts automatically when I turn on the computer.”  

These requests are enough for a technical helper to complete the setup.

---

## Manuals and guides that are appropriate
A technical helper can rely on:

- the official Ollama installation guide for the operating system  
- the Open WebUI documentation for connecting to Ollama  
- the model documentation for any special requirements  

These guides are written for general users and do not require deep expertise.

---

## Alternatives if the computer is older or weaker
Different computers handle AI models differently. A helper can choose:

- **Small models** for older laptops  
- **Medium models** for typical home desktops  
- **Large models** for gaming PCs or workstations  

If the computer cannot run models locally, alternatives include:

- using cloud‑based AI services  
- using a remote computer in the home  
- using a lightweight model that fits the hardware  

The non‑technical user does not need to choose; the helper selects the appropriate option.

---

## How much Open WebUI supports other systems
Open WebUI can connect to several types of AI backends:

- **Ollama** for local models  
- **OpenAI‑style APIs** for cloud models  
- **LitGPT servers** if someone runs a custom model  
- **LM Studio** if installed as a local backend  
- **ChatGPT or Copilot** through API keys  

This means the user can switch between:

- local models  
- cloud models  
- fine‑tuned models  
- experimental models  

without changing the interface.

---

## How much each component is needed
- **Ollama** is needed for running local models.  
- **Open WebUI** is needed for a simple, browser‑based interface.  
- **LitGPT** is optional and only needed if someone wants to fine‑tune models.  
- **LM Studio** is optional and provides another local backend.  
- **ChatGPT and Copilot** are optional cloud services.  

A non‑technical user only needs Ollama and Open WebUI for a complete local setup.

---

## Role diagram: how the setup works for a family

```mermaid
flowchart TD
    A[Mother uses browser interface] --> B[Open WebUI]
    B --> C[Backend selection: Ollama or cloud API]
    C --> D[Model runs on chosen backend]
    D --> E[Response returned to Open WebUI]
    E --> A[Mother continues chatting]

    F[Child or friend installs Ollama] --> C
    G[Child or friend configures Open WebUI] --> B
```

# Setting up LitGPT, using generic “initial cards”, converting Anki decks to JSONL, and turning all daily commands into a GUI

## LitGPT setup in practical terms
LitGPT is a framework for running and fine‑tuning language models. A helper installs it once by following the official instructions for the operating system. After installation, LitGPT can:

- run a model  
- fine‑tune a model  
- serve a model through an API endpoint  

A non‑technical user does not interact with LitGPT directly. They only use the GUI that the child or helper builds.

---

## Using generic “initial cards” for LitGPT
LitGPT supports training and fine‑tuning with JSONL files. These files contain:

- an instruction  
- an input (optional)  
- an output  

Generic “initial cards” are simply ready‑made JSONL entries that act as the model’s starting examples. They can be:

- downloaded from public sources  
- written manually  
- generated from existing notes or flashcards  

LitGPT treats these entries as training data. The helper places them in the correct folder, and LitGPT uses them during fine‑tuning.

---

## Converting Anki decks to JSONL
Anki decks can be exported as:

- `.apkg` files  
- `.csv` files  

A helper or friend can convert them to JSONL using a Python script. The script reads each card and produces entries that LitGPT understands. The conversion process follows the same pattern described earlier:

- a Python script with a `main` entry point  
- a command that runs it  
- a GUI button that launches the command  

This allows the mother to convert decks without touching the command line.

---

## Connecting these tasks to a GUI
A Visual Basic form can provide:

- a button to choose an Anki deck  
- a button to convert it to JSONL  
- a button to start LitGPT fine‑tuning  
- a button to run the fine‑tuned model  
- a button to open the inference interface  

Each button triggers a single event. The event launches the appropriate command. The mother interacts only with the GUI.

---

## Role diagram: how LitGPT, conversion scripts, and the GUI interact

```mermaid
flowchart TD
    A[Mother uses GUI buttons] --> B[Visual Basic form]
    B --> C[Button triggers conversion or training]
    C --> D[Process.Start runs Python or LitGPT command]
    D --> E[Conversion to JSONL or model fine-tuning]
    E --> F[Model ready for inference]

    G[Child builds GUI] --> B
    H[Friend or sibling writes Python conversion scripts] --> D
    I[Helper installs LitGPT] --> E
```

# Setting up LitGPT, using generic starter cards, converting Anki decks to JSONL, and turning all recurring commands into a GUI

## Installing LitGPT in practical terms
LitGPT is installed once by a helper who follows the official instructions for the operating system. The installation provides:

- the LitGPT command runner  
- configuration files  
- training and inference scripts  
- the ability to serve a model through an API endpoint  

A non‑technical user does not interact with LitGPT directly. After installation, all actions can be triggered through a GUI.

---

## Using generic starter cards (“initial cards”)
LitGPT fine‑tuning uses JSONL files. These files contain entries such as:

- an instruction  
- optional input  
- the expected output  

Generic starter cards are simply ready‑made JSONL entries that act as the model’s initial examples. They can be:

- downloaded from public sources  
- created manually  
- generated from existing notes or flashcards  

A helper places these JSONL files in the correct folder. LitGPT uses them automatically during fine‑tuning.

---

## Converting Anki decks to JSONL
Anki decks can be exported as `.apkg` or `.csv`. A Python script can convert them to JSONL. The script typically:

- reads each card  
- extracts the front and back  
- writes a JSONL entry for each pair  

The script includes a `main` entry point so it can be run directly.  
A child can connect this script to a GUI button, so the mother selects a deck and the conversion happens automatically.

---

## Connecting LitGPT tasks to a GUI
A Visual Basic form can provide:

- a button to choose an Anki deck  
- a button to convert it to JSONL  
- a button to start fine‑tuning  
- a button to run the fine‑tuned model  
- a button to open the inference interface  

Each button triggers a single event. The event launches the appropriate command.  
The mother interacts only with the GUI.

---

## Role diagram: how LitGPT, conversion scripts, and the GUI interact

```mermaid
flowchart TD
    A[Mother uses GUI buttons] --> B[Visual Basic form]
    B --> C[Button triggers conversion or training]
    C --> D[Process.Start runs Python or LitGPT command]
    D --> E[Conversion to JSONL or model fine-tuning]
    E --> F[Model ready for inference]

    G[Child builds GUI] --> B
    H[Friend or sibling writes Python conversion scripts] --> D
    I[Helper installs LitGPT] --> E
```

This diagram shows the separation of roles:

- The mother uses the GUI  
- The child builds the GUI  
- A friend or sibling writes conversion scripts  
- A helper installs LitGPT  

The mother never sees the command line.

---

## Autoloading tasks at startup
A GUI program can:

- start automatically when Windows starts  
- load the last used model  
- show buttons for daily tasks  
- remember file locations  

This removes the need for repeated setup. The mother opens the computer and the interface is ready.

---

## Summary
LitGPT is installed once by a helper. Generic starter cards are JSONL entries that LitGPT uses for training. Anki decks can be converted to JSONL through Python scripts. A child can wrap all commands in a Visual Basic GUI with buttons and dialogs. The mother interacts only with the GUI, while helpers handle installation and configuration.
