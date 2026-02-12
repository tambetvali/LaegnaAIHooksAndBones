# Chapter 1 — Anki Decks and AI Q&A Datasets: A Structural Comparison  
*A practical guide to understanding how human flashcard systems mirror AI learning systems*

If you’ve ever used Anki, you already understand one of the deepest parallels between human learning and AI learning. Anki is a structured, spaced‑repetition system built around **decks** and **flashcards**. AI training datasets — especially Q&A datasets — follow the same logic.

Both systems rely on:

- clear questions,  
- clear answers,  
- structured organization,  
- and repeated exposure.

This chapter explains how Anki decks map directly to AI Q&A datasets, and why the same preparation process applies to both.

---

## 1. Decks: Human Containers vs. AI Containers

In Anki, a **deck** is a named container for flashcards.  
In AI, a **dataset** or **corpus** is the same thing.

Both serve as:

- a boundary,  
- a topic area,  
- a context,  
- and a retrieval space.

Anki decks may be nested (“Physics → Mechanics → Forces”).  
AI datasets may be nested (“physics/mechanics/forces.jsonl”).

Different Anki GUIs display decks differently:

- Desktop: hierarchical tree  
- Mobile: flat list with slashes  
- Web: grouped sections  

AI systems do the same:

- some store datasets as folders,  
- some as tags,  
- some as vector collections.

But the concept is identical:  
**a deck is a structured space of meaning.**

---

## 2. Flashcards: Human Q&A vs. AI Q&A

A flashcard in Anki:

- **Front:** question  
- **Back:** answer  

A training example in AI:

- **Q:** prompt  
- **A:** completion  

The structure is the same.

Anki adds:

- formatting,  
- images,  
- audio,  
- cloze deletions,  
- scheduling.

AI adds:

- embeddings,  
- tokenization,  
- retrieval,  
- fine‑tuning.

But the core unit — the Q&A pair — is identical.

---

## 3. The Pre‑Work: The Shared Foundation

Whether you are preparing Anki cards or AI training data, the process is the same:

1. Create the question.  
2. Create the answer.  
3. Test whether it works.  
4. Refine wording.  
5. Remove unclear or useless cards.  
6. Add examples or variations.  

This is why Anki is such a powerful metaphor for AI learning:  
**the preparation is identical.**

---

## 4. Three Ways to Create Cards (Human or AI)

### 4.1. Cards Generated From Documents  
You extract Q&A pairs from:

- notes,  
- summaries,  
- explanations,  
- definitions,  
- examples.

This is the same process used to build RAG datasets.

### 4.2. Cards Created as Lesson Material  
You:

- name the lesson,  
- create the cards manually,  
- or scan physical cards.

This mirrors how domain experts create fine‑tuning datasets.

### 4.3. Cards Generated Automatically  
You let:

- AI generate cards from text,  
- scripts extract definitions,  
- simulations generate numeric cases.

This mirrors synthetic dataset generation for AI.

---

## 5. Why This Matters

Anki decks and AI datasets are two versions of the same idea:

- **structured knowledge**,  
- **expressed as Q&A**,  
- **organized into decks**,  
- **tested repeatedly**,  
- **refined over time**.

Understanding one helps you understand the other.

---

# Chapter 2 — AI‑Ready Formats: What Works, What Fails, and Why  
*A practical guide to choosing formats that are human‑testable, GUI‑accessible, reusable, and suitable for AI systems*

When preparing knowledge for AI, the format matters. Some formats are excellent for both humans and machines. Others are useful only internally. Some are outright unsuitable.

This chapter explains which formats work as **standard, GUI‑accessible, human‑testable, reusable AI formats**, and which formats fail to meet those criteria.

---

## 1. Formats That Work Well for Both Humans and AI

These formats are readable, editable, testable, and reusable.

### 1.1. Markdown (`.md`)
**The gold standard.**

- Human‑readable  
- Version‑controllable  
- Easy to annotate  
- Easy to convert  
- Perfect for RAG  
- Perfect for Q&A cards  
- Works in any GUI editor  

Markdown is the closest thing to a universal AI‑ready format.

### 1.2. Plain Text (`.txt`)
Simple, durable, universal.

- No formatting  
- No dependencies  
- Easy to parse  
- Easy to embed  

Perfect for raw Q&A pairs.

### 1.3. JSON / JSONL
Ideal for structured datasets.

- Key/value pairs  
- Easy to parse programmatically  
- Works for fine‑tuning  
- Works for RAG metadata  
- Human‑readable with a decent editor  

JSONL is the standard for AI training.

### 1.4. CSV / TSV
Great for tables and structured fields.

- Easy to open in Excel  
- Easy to parse  
- Good for numeric or categorical data  

Not ideal for long text, but excellent for structured knowledge.

### 1.5. Static HTML / Static Websites
Perfect for RAG ingestion.

- Predictable structure  
- Easy to crawl  
- Easy to convert to Markdown  
- Human‑testable in any browser  

This is why many documentation systems export to static sites.

---

## 2. Formats That Are Useful but Require Conversion

These formats are good for humans but need preprocessing for AI.

### 2.1. PDF
Readable, portable, but:

- inconsistent structure  
- difficult to parse  
- requires OCR for scanned pages  

AI can use PDFs, but only after conversion.

### 2.2. Word Documents (`.docx`)
Good for writing, but:

- heavy  
- XML‑based  
- inconsistent formatting  

Best converted to Markdown.

### 2.3. Images with Text
Useful for diagrams, but:

- require OCR  
- require alt‑text or summaries  
- not directly AI‑ready  

Always pair with a Markdown description.

---

## 3. Formats That Fail as AI‑Ready Knowledge

These formats are not suitable for human‑simulation or AI ingestion.

### 3.1. Raw Database Dumps (`.sql`, `.sqlite`, `.db`)
AI cannot meaningfully learn from:

- normalized tables  
- foreign keys  
- binary blobs  
- schema‑heavy structures  

These must be converted into:

- text summaries,  
- Q&A pairs,  
- or structured JSON.

### 3.2. Proprietary CMS Internal Formats
These include:

- internal XML  
- proprietary JSON  
- hidden metadata  
- unpublished schemas  

They are not meant for human reading or AI ingestion.

### 3.3. Dispersed, Unstructured CMS Content
CMS systems often store content as:

- fragments  
- widgets  
- blocks  
- templates  
- partials  

AI cannot reconstruct meaning without a unified export.

### 3.4. Formats Without Human‑Testability
If a human cannot:

- read it,  
- test it,  
- verify it,  
- or simulate it,  

then it is not suitable as a reusable AI knowledge format.

---

## 4. The Rule of Reusability

A format is AI‑ready if:

- a human can read it,  
- a human can test it,  
- a GUI can display it,  
- an AI can parse it,  
- and it can be reused in future systems.

Markdown, JSON, and static HTML meet all criteria.  
Database dumps, proprietary CMS formats, and dispersed content do not.

---

# Chapter 3 — Using AI to Maintain, Clean, and Expand Your Anki Decks  
*A practical guide to integrating AI into your flashcard workflow*

AI can be a powerful assistant in managing your Anki decks — not by replacing your thinking, but by supporting it.

This chapter explains how AI can help you maintain, clean, and expand your decks while keeping you in control.

---

## 1. Cleaning Existing Decks

AI can help you:

- rewrite unclear questions,  
- simplify answers,  
- split overloaded cards,  
- merge duplicates,  
- add missing context,  
- remove irrelevant cards.

You remain the editor.  
AI is the assistant.

---

## 2. Expanding Decks With New Material

AI can:

- generate new cards from your notes,  
- extract Q&A pairs from documents,  
- create variations of existing cards,  
- generate examples,  
- create cloze deletions,  
- propose new sub‑decks.

You decide which cards to keep.

---

## 3. Converting Decks Into AI‑Ready Formats

Your Anki decks can be exported to:

- CSV  
- JSON  
- text  
- Markdown (with plugins)  

These formats can be used for:

- RAG datasets,  
- fine‑tuning datasets,  
- domain‑specific assistants,  
- knowledge bases.

Your flashcards become reusable knowledge.

---

## 4. Using AI to Generate Synthetic Cards

AI can generate:

- numeric examples (physics, math),  
- scenario variations,  
- edge cases,  
- conceptual explanations,  
- analogies,  
- diagrams (with descriptions).

This mirrors synthetic dataset generation in AI training.

---

## 5. The Human‑AI Partnership

AI does not replace your judgment.  
It amplifies your ability to:

- organize,  
- clarify,  
- expand,  
- and refine knowledge.

You remain the teacher.  
AI is the assistant who helps you build a better deck.

---

# Final Thoughts

Anki decks, Markdown flashcards, and AI Q&A datasets are all versions of the same idea:

- structured knowledge,  
- expressed as questions and answers,  
- organized into decks,  
- tested repeatedly,  
- refined over time.

Whether you are learning yourself or teaching an AI, the process is the same:

**Ask clearly.  
Answer clearly.  
Organize meaningfully.  
Repeat until it becomes knowledge.**

# Machine‑Learning Data: From Real‑Life Tables to AI‑Ready Knowledge  
*A practical chapter using the “concert business” example*

Machine learning becomes far easier to understand when you connect it to something concrete. Imagine you organize concerts. Over time, you’ve collected a table of your experience — a simple spreadsheet with fields describing each event.

This table already contains everything a machine‑learning system needs:  
**inputs (Q fields)** and **outputs (A fields)**.

---

# 1. The Experience Table: Q Fields and A Fields

Your table might look like this:

## Q fields (inputs)
These describe the situation — the “question” part.

- **Where** the concert took place (`concert hall`, `club`, `outside`, etc., 10 types)
- **Ticket price**
- **Length** of the concert (`30 minutes`, `1 hour`, `2 hours`)
- **Solo** or **shared** concert (`solo = 1`, `shared = 0`)

## A fields (outputs)
These describe what happened — the “answer” part.

- **How much you earned**
- **How much you spent**
- **Whether any financial problems occurred**

This is a perfect Q → A dataset.

---

# 2. The Machine‑Learning View: Turning Q and A Into a Function

Machine learning sees your table as a function:

$$
Q \rightarrow A
$$

Where:

- $f_1$ describes the inputs (Q fields)  
- $f_2$ describes the outputs (A fields)

So the system tries to learn:

$$
f_1(\text{where, price, length, solo}) = f_2(\text{earned, spent, problems})
$$

This is the **core idea**:  
AI tries to discover the relationship between the situation and the outcome.

---

# 3. A Simple (But Weak) Linear Model

You can express this relationship in a simple linear form.  
Because this is block math, it must be outside any list:

$$
\text{earned} = x_1 \cdot \text{where} + y_1 \cdot \text{price} + z_1 \cdot \text{length} + t_1 \cdot \text{solo}
$$

$$
\text{spent} = x_2 \cdot \text{where} + y_2 \cdot \text{price} + z_2 \cdot \text{length} + t_2 \cdot \text{solo}
$$

$$
\text{problems} = x_3 \cdot \text{where} + y_3 \cdot \text{price} + z_3 \cdot \text{length} + t_3 \cdot \text{solo}
$$

This gives you **12 unknowns**:

- $x_1, y_1, z_1, t_1$  
- $x_2, y_2, z_2, t_2$  
- $x_3, y_3, z_3, t_3$

A machine‑learning algorithm can optimize these numbers to best fit your past data.

This model is simple — too simple for real business — but it illustrates the idea:

- Q fields become numeric or categorical inputs  
- A fields become numeric or categorical outputs  
- The algorithm finds the best mapping between them

---

# 4. Real‑World Models: Using Business Templates

In practice, you don’t want to invent your own formulas.  
You want to use **existing business templates**, such as:

- company size classes  
- revenue models  
- cost structures  
- risk estimation formulas  
- profitability equations  

These templates already exist in:

- business school materials  
- accounting frameworks  
- financial analysis textbooks  

AI can learn which template fits your data best.  
This gives you a **meaningful**, **interpretable**, and **domain‑correct** model.

---

# 5. Putting This Into an Anki Deck

Anki is a perfect place to store:

- the Q fields  
- the A fields  
- the meaning of each field  
- the formulas  
- the examples  
- the unknowns  
- the solved cases  

Why?

Because Anki forces you to express everything as **clear Q&A pairs**.

### Example cards (inline math only):

- **Front:** What are the Q fields in the concert dataset?  
  **Back:** $where$, $price$, $length$, $solo$.

- **Front:** What does the machine‑learning function try to learn?  
  **Back:** The mapping $Q \rightarrow A$.

- **Front:** How many unknowns are in the linear model?  
  **Back:** $12$ coefficients ($x_1$–$t_3$).

This makes the system:

- human‑testable  
- easy to revise  
- easy to expand  
- easy to export  
- easy to reuse for AI

---

# 6. Using the Table Directly for Machine Learning

Your raw table is already machine‑learning data.

You can:

- feed it into a regression model  
- use it for classification (`problems = yes/no`)  
- use it for clustering (`types of concerts`)  
- use it for forecasting (`future earnings`)

The table is the **ground truth**.

---

# 7. Using Templates for AI Learning

You can also create a **template card** that describes the function:

**Front:**  
What is the general form of the Q → A function?

**Back:**  
A mapping from $(where, price, length, solo)$ to $(earned, spent, problems)$, expressed as a business formula or learned model.

GPT‑style models can learn this in **textual format**, which allows:

- reasoning  
- explanation  
- contextual understanding  
- symbolic manipulation  
- example generation  

This is different from numeric machine learning, but complementary.

---

# 8. Machine Learning Systems and Anki: How They Connect

Machine‑learning systems prefer:

- numeric fields  
- structured tables  
- known formulas  
- unknown coefficients  
- optimization

Anki prefers:

- text  
- Q&A  
- human‑readable structure  
- examples  
- explanations

But both systems benefit from the same preparation:

- clear fields  
- clear definitions  
- clear examples  
- clear relationships  

And both systems can use the same **source data**.

---

# 9. Converting Anki to Machine‑Learning Data

Anki stores its data in **SQLite**, which means:

- you can extract fields  
- you can export decks  
- you can convert them to CSV or JSON  
- you can feed them into ML systems

Tools like:

- Python  
- SQL no‑code tools  
- SpaCy  
- AI extraction scripts  

can convert Anki cards into structured data.

This is especially useful when:

- you create cards with fields  
- you embed numeric examples  
- you store templates  
- you store solved cases

---

# 10. Creating Cases and Solutions: The Generic Pattern

To make your dataset useful for both humans and AI:

1. **Define the Q fields**  
   (inputs, conditions, situation)

2. **Define the A fields**  
   (outcomes, results, consequences)

3. **Create examples**  
   (rows in your table)

4. **Create templates**  
   (the general form of the function)

5. **Create unknowns**  
   (coefficients, parameters, weights)

6. **Create solved cases**  
   (examples where the unknowns are filled)

7. **Store everything in both formats**  
   - human‑readable (Anki, Markdown)  
   - machine‑readable (CSV, JSON, SQL)

This gives you a **dual‑use dataset**:

- humans can study it  
- AI can learn from it  
- both can reason about it  
- both can reuse it in the future

---

# Final Thoughts

Your concert table is more than a spreadsheet.  
It is:

- a machine‑learning dataset  
- a Q&A deck  
- a business model  
- a set of examples  
- a set of unknowns  
- a set of solutions  
- a reusable knowledge base

By expressing it in both **Anki** and **AI‑ready formats**, you create a system that:

- humans can understand  
- AI can learn  
- and both can improve over time

This is the essence of modern knowledge engineering.

# Domain‑Based Machine Learning: From Small Business to Scalable Models  
*A practical explanation using a standard small‑business database*

To understand domain‑based machine learning, it helps to start with something familiar: a small business with a simple, structured database. The same principles scale to large companies, public institutions, or even individuals tracking personal finances.

---

# 1. A Standard Small‑Business Case

Imagine a small business — a bakery, a repair shop, a concert organizer, a farm stand.  
They typically maintain a simple database with tables like:

- **Sales**  
  - date  
  - product or service  
  - price  
  - quantity  
  - location or channel  
  - customer type  

- **Costs**  
  - materials  
  - labor  
  - rent  
  - utilities  
  - transportation  

- **Events or Jobs**  
  - duration  
  - staff involved  
  - equipment used  
  - external partners  

This is the same structure used by:

- freelancers  
- mid‑size companies  
- large enterprises (just with more fields)  

The *shape* of the data is stable across scales.

---

# 2. A Standard, Scalable Question

A question that works for small and large businesses alike:

**“Given the conditions of an event or job, what will the financial outcome be?”**

This question scales because:

- a freelancer asks it for a single job  
- a small business asks it for weekly planning  
- a corporation asks it for forecasting across regions  
- a government asks it for economic modeling  

The structure is always:

$$
Q \rightarrow A
$$

Where:

- $Q$ = conditions, inputs, context  
- $A$ = outcomes, results, consequences  

This is the universal shape of machine‑learning problems.

---

# 3. General AI vs. Machine Learning vs. Domain‑Based ML

To understand domain‑based ML, we must contrast it with two other approaches.

---

## 3.1. General AI (Deep Learning)

Deep learning uses **universal, balanced mathematical primitives**:

- matrix multiplication  
- bias addition  
- activation functions  

These operations are extremely general.  
A deep network can approximate almost any function.

Deep learning is:

- **holistic** (field‑based, not symbolic)  
- **high‑dimensional** (2D matrices, often huge)  
- **agnostic to domain**  
- **powerful but hard to interpret**  

It is excellent for:

- images  
- audio  
- natural language  
- complex nonlinear patterns  

But it does not naturally express:

- business formulas  
- accounting logic  
- domain‑specific equations  

It *can* learn them, but the meaning is buried inside matrices.

---

## 3.2. Generic Machine Learning (Classical ML)

Classical ML uses **school‑level mathematical templates**:

- linear regression  
- polynomial regression  
- logistic regression  
- decision trees  
- SVMs  

These operate on **1D vectors**:

- variables $v_1, v_2, v_3, \dots$  
- unknowns $x_1, x_2, x_3, \dots$  

They are:

- efficient  
- interpretable  
- stable  
- mathematically balanced  

A good ML model:

- handles negative numbers  
- handles scaling  
- handles precision changes  
- remains stable when vector size increases  

A *bad* ML formulation:

- forbids negative values  
- collapses when precision changes  
- becomes unstable when adding variables  
- cannot scale to larger datasets  

---

## 3.3. Domain‑Based Machine Learning

Domain‑based ML uses **the formulas of the domain itself**:

- business equations  
- climate models  
- agricultural yield formulas  
- physics relationships  
- financial ratios  
- risk models  

These formulas have three key properties:

### 1. **Balanced input → output relationships**  
Changing inputs smoothly changes outputs.  
This is essential for learning.

### 2. **Linear or linearizable structure**  
Even complex formulas often have a linear core.  
This makes them stable and scalable.

### 3. **Scalable meaning**  
If you add parameters:

- the formula still works  
- the interpretation still works  
- the theory still works  

This is what makes it *domain‑based* rather than *ad‑hoc*.

---

# 4. Why Domain‑Based ML Works

Domain‑based ML succeeds because:

- the formulas already exist  
- the relationships are meaningful  
- the unknowns correspond to real‑world quantities  
- scaling preserves meaning  
- the model fits into existing theory  

For example:

- A small bakery uses a cost‑of‑goods formula.  
- A large chain uses the same formula with more parameters.  
- A national retailer uses the same formula with regional adjustments.  

The *structure* is identical.

---

# 5. When You Are “Just Using ML to Solve a Formula”

You are simply using ML to solve a formula when:

### 1. **The formula is not balanced**  
Example:  
A small company’s variable $v_3$ ranges from $0.00001$ to $0.00014$,  
but a large company’s $v_3$ ranges from $30$ to $40$.

ML will struggle because the meaning does not scale.

### 2. **You cannot extend the formula**  
Example:  
Your company grows, but your old formula cannot incorporate:

- new product lines  
- new cost structures  
- new risk factors  

A domain‑based formula would scale naturally.

### 3. **The solution is not standard**  
If your formula is unique and not connected to:

- business theory  
- accounting standards  
- economic models  

then ML cannot “learn the context.”  
It only fits numbers, not meaning.

### 4. **The meaning does not scale**  
Example:  
You have a field called “connection with organization X.”  
But:

- for you it means “customer relationship”  
- for a government it means “regulatory oversight”  
- for a partner it means “strategic alliance”

The variable name is the same, but the meaning is not.  
This breaks domain learning.

---

# 6. Why Domain‑Based ML Is the Right Approach

Domain‑based ML:

- uses formulas that already exist  
- scales with business size  
- preserves meaning  
- allows comparison across companies  
- integrates with theory  
- produces interpretable results  
- avoids paradigm shifts  

It is the bridge between:

- **small business intuition**  
- **large enterprise analytics**  
- **scientific modeling**  
- **AI automation**

This is why domain‑based ML is the most stable, scalable, and meaningful form of machine learning for real‑world use.

---

# Final Thoughts

A small business database is not “toy data.”  
It is a micro‑version of the same structures used by:

- corporations  
- governments  
- scientific institutions  

Domain‑based machine learning recognizes this continuity.  
It uses the formulas of the domain — business, climate, science — to create models that:

- scale  
- remain meaningful  
- integrate with theory  
- and learn smoothly  

This is how small‑business data becomes part of a general, scalable, intelligent system.

# Appenix

***You might get some data for initial tasks for some of the text - this is not part of the content, but clarification and somewhat "draft format" as it's was used to produce some chapters before; it still contains some of my rich data:***

# Appendix: Original Instructions and Prompts

## Section 1 — Concert Machine‑Learning Example  
*(From “Imagine you make concerts…” to “…either with fields or field expressions on card.”)*

Imagine you make concerts and you have managed to create a table of your experience, which has:
- Q fields:
  - Where (concert hall, outside, etc., 10 types)
  - Ticket price
  - Length (30 minutes, hour, 2 hours)
  - Solo concert or other artists
- A fields:
  - How much you earned
  - How much you spent
  - Were there any financial problems in any related process

Machine Learning:

You create a function form:
- Q = A
  - Q: f_1(where, price, length, solo)
  - A: f_2(earned, spent, problems)
  - You can associate each field is text or number, and have final form:
    - Q = A => f_1(where, price, length, solo) = f_2(earned, spent, problems)
  - There is *possible direct solution* - AI learns the function f_1; it will give you some form of output, such as linear regression form of this equation, but you use yours.
- Unknowns for an AI
  - Mostly, you can now create the function form with unknowns:
    - Q = A
      - f_1(where, price, length, solo) =
        - x1 * where + y1 * price + z1 * length + t1 * solo => earned
        - x2 * where + y2 * price + z2 * length + t2 * solo => spent
        - x3 * where + y3 * price + z3 * length + t3 * solo => problems
      - While this is stupid function form and almost definitely not yield very good solutions, the machine learning algorithm would file x, y, z and t from 1 to 3 with 12 numbers after optimization; this algorithm is linear and thus while not efficient, easy to optimize towards it's maximum efficiency. Notice that the numbered variables in this new format are A, and both input and output of the function are fields to Q.
      - For real, you want to use the calculation template from your school, or business school: one which describes, for example, possible company sizes (size classes), and then gives the equation to resolve monetary situation - an AI would figure out such company size class, which suits your actual accounting, based on the past table.

This is useful to put this into Anki deck:
- You can add fields and values to Q&A
  - You can use this final table directly for machine learning
  - You can create template, which shows the Q&A meaningfully:
    - A GPT can learn them in textual format;
      - and it can also learn the set where generated unknowns are already met.
      - this allows it to enable this machine learning feature, as well as reason about the context.
    - Machine learning system likes the unknowns and the function form, and suits with your table. It does not read Anki textual format, but you can prefer Anki to raw table - it can read the fields with SQLite-compatible interface (it's easy to convert SQLite into web-served format or generate a file, for example with Python or many SQL no-coders or existing systems, and there are many SQL-related systems for simple field extraction); some of them might support anki or SQLite. The other way is to figure out Anki export formats, whether and how they support fields. The system to convert visual cards to raw data is SpaCy or it can be an AI task, in case you *create* the cards in initial Anki format, either with fields or field expressions on card.

---

## Section 2 — Domain‑Based Machine Learning Instructions  
*(From “Standard small-business case…” to “…it must not be filled in, what means ‘connection’.”)*

### Standard small-business case with their typical database
### A standard, generally recognizable and preferrably somewhat scalable question (i.e. similar happens to large company or individual with no much paradigm shifts)
### To turn it to proper domain-based machine learning (express and explain the term):
  - General AI:
    - Deep Learning uses very universal, balanced formulae - matrix+bias calculation is math primitive, expressing it's ultimate harmonic balance; most generally, in known automatable and optimal math, this is simple syntax to express many different functions with equal probability of fit and simplicity, for example typical math problem does not escape the scale or is itself very complex. Standard science tools can be used for operations on results, altough it's hard to read or to give meaning to it's parts (holistic, field-based, rather than rational and symbol-based). DL uses 2D matrix, often large.
    - Machine Learning uses very typical formats we learn in school as generic templates - linear regression, polynominals, ones where typically your variables v1, v2, v3, ... come along with unknowns x1, x2, x3, ...; it's also "learning" and "generic" in sense that these are typical 1D vectors, which are most efficient to resolve; also the solutions have mathematical balance and efficiently scale to random distribution of expressions in such linear complexity.
      - For example, *not* generic learning would
        - not solve some condition,
          - like lacking minus numbers in it's general form;
          - like giving the minus number area small probability, distribution and scale, so that optimizer reaches them inefficiently or precision is not stable;
        - not scope with a number:
           - you could not change the precision, remaining in stable area, by changing the size of vector (1D machine learning) or matrix (2D deep learning), and getting stable benefit from the scale.
           - in deep learning, if you scale it into *as big as you get into*, before it disturbs other space-takers, is typical for data you *won't read manually*, but machine learning will give your *high school expressions*, like linear equation or polynominal systems - you generally thrive with *shortest expressions, which are still expressive*, and you might not be interested in all digits even in this.

Domain learning associates:
- The business, farming, climate, science formulae which turns this into *domain-based machine learning* is general in your domain:
  - Climate or business formulae has balanced input=>output relationship; changing the learnt data (unknowns) smoothly, by given steps, also remains stable and smooth in output.
    - It's rather linear, or has at least some linearizable properties (where the latter can be quite complex, and linear can be quite simple and straightforward to implement and understand - often the values your business already has for it's critical eqations, and what follows is not exception in this)
    - It scales linearly in nD - if you add parameters, rows or columns in same format, the value of equation will raise in case you need more complex or precise solution, you would not reinvent the formulae
    - This is standard solution in your domain or business or climate vector: theoretic capability adds to every aspect, and to "learn", very often means to bring into general consciousness, parallel, contradicting and useful patterns
      - The meaning scales as well: for example, same equation with more or less parameters compares you with other business, and even fits the formulaes they actually use and publish, or is a direct conversion or implication. Then, it also *learns generally in context*, altough it's domain specific - for atom energy, your business formulae might not suit, while the general ml or dl might resolve it as easily and closely with it's general form.

You are simply using ML to solve a formulae if:
- It's not balanced: for example, for small companies you have to balance unknown v3 between 0.00001 and 0.00014, while for big companies it's between 30 and 40
- You cannot extend it: for example, when your company is growing, you have other standard formulae, or you compare with other companies not based on math, but intuition - you say 72, they say 45, but it's another unit and you don't see where the paradigm shifts. So it does not "learn the context" (you lose it there). Generic formulae learns the context as system without explicitly being aware - your unknowns fit the contextual theory.
- This is not standard solution: to "learn" means that it gives you a piece of data, which you can use tracking the implications *from now on, automatically, more or less*: for example, you download random Prolog program, give it your equation form (unknowns, base), and are already connected to theories - this means general learning, because in *prolog tautological system*, you can ask random questions, and they are learnt; if you have unique math framework - unless you are very serious about it and it's development, integrations, conversions etc., the prolog would *learn unrelated data*, thus *not learn*: it's not an intuition, but an abstract symbol.
- The meaning does not scale: for example, you state that you have "connection with political organization x", when you fill a form; but your government has same connection with same function, but the connection is different. Rather, you have "end user connection with this IT company" and another might be companion, or even "friend" in a sense. While linguistic form might be similar, the functional form must properly scale and not reuse same variable for other reasons, or you *can not extend the theory*, ultimately, because *it must not be filled in, what means "connection"*.
