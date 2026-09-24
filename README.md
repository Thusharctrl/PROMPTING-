# Prompt Engineering Techniques — Quick Reference

A practical cheat sheet for the prompting techniques and shorthand terms covered in this session.

> **Note:** Terms such as **ELI5, ELI10, PLANIFY, STORYIFY, POETIFY, REMIX, and T-TR** are useful prompting labels, but they are not all standardized industry terminology. Their exact meaning can vary by instructor, course, or prompting framework. For **T-TR** especially, verify the definition used in your session.

---

## 1. Prompting by Examples and Instructions

These techniques mainly control **how much guidance or context the model receives**.

| Technique | Description | Example |
|---|---|---|
| **Zero-shot** | Ask the model to perform a task **without providing an example**. | `Translate "Hello" to Spanish.` |
| **One-shot** | Provide **one example** showing the desired pattern, then ask for a new result. | `Cat → Animal. Rose → ?` |
| **Few-shot** | Provide **multiple examples** so the model can infer the expected pattern. | `Cat → Animal; Rose → Plant; Eagle → ?` |
| **Role-based prompting** | Assign the model a **role or expertise** to guide its perspective and response style. | `Act as a Python tutor and explain lists to a beginner.` |

### Quick memory trick

- **Zero-shot** → No example
- **One-shot** → One example
- **Few-shot** → Several examples
- **Role-based** → Give the model a role

---

## 2. Explanation and Understanding Prompts

These techniques control **how the model explains information**.

| Technique | Description | Example |
|---|---|---|
| **ELI5** | Explain something using extremely simple language, as if explaining to a young child. | `Explain APIs ELI5.` |
| **ELI10** | Explain something at roughly a 10-year-old level: simple, but with slightly more detail than ELI5. | `Explain recursion ELI10.` |
| **BREAKDOWN** | Split a complex concept into **smaller, manageable parts**. | `Break down how a REST API works.` |
| **DEMYSTIFY** | Remove confusion around a topic and make the underlying idea clearer. | `Demystify neural networks.` |
| **SIMPLIFY** | Keep the core meaning while making the language or explanation easier to understand. | `Simplify this research paper.` |
| **ANALOGY** | Explain a concept by comparing it with something familiar. | `Explain RAM using a desk analogy.` |
| **VISUALIZE** | Describe a concept in a way that helps the reader **picture the process or structure**. | `Visualize how a CPU executes an instruction.` |
| **T-TR** | In your session, this was described as **Think → Translate → Respond**: reason about the concept, translate it into understandable language, then answer. | `Use T-TR to explain backpropagation to a beginner.` |

### Important distinctions

**SIMPLIFY ≠ CONDENSE**

- **Simplify** → make it easier to understand
- **Condense** → make it shorter

**BREAKDOWN ≠ ANALOGY**

- **Breakdown** → split the concept into components
- **Analogy** → explain it through comparison

---

## 3. Summarization and Compression Prompts

These techniques reduce information while changing the **level of detail or output length**.

| Technique | Description | Example |
|---|---|---|
| **ABSTRACT** | Give the **high-level summary** while leaving out lower-level details. | `Abstract this system design in 5 sentences.` |
| **CONDENSE** | Make the content **shorter while preserving the important information**. | `Condense this article to 100 words.` |
| **ESSENCE** | Extract the **central idea or core message**. | `Give me the essence of this paper.` |
| **1-LINER / 1LINEAR** | Reduce the answer to **one sentence**. | `Explain TCP in one line.` |
| **IN 3 BULLETS** | Reduce the answer to **three key points**. | `Explain TCP in 3 bullets.` |

### Quick memory trick

- **Abstract** → High-level summary
- **Condense** → Shorter version
- **Essence** → Core idea
- **1-liner** → One sentence
- **3 bullets** → Three key points

---

## 4. Style and Transformation Prompts

These techniques change **how the information is expressed**.

| Technique | Description | Example |
|---|---|---|
| **PLANIFY** | Transform an idea into a **structured plan, roadmap, or sequence of actions**. | `Planify my Python learning journey.` |
| **FORMALIZE** | Rewrite content in a **formal, professional, or academic style**. | `Formalize this message to my professor.` |
| **CASUALIZE** | Rewrite content in a **casual, natural, conversational style**. | `Casualize this email.` |
| **STORYIFY** | Turn information into a **story or narrative**. | `Storyify the history of the Internet.` |
| **POETIFY** | Rewrite content using **poetic language or a poem-like style**. | `Poetify this message.` |
| **MIMIC** | Produce new content that follows the **style, structure, or pattern of a supplied reference**. | `Mimic the structure of this example and write one for my project.` |

### One idea, six transformations

Original:

> `I need to learn Python.`

**PLANIFY**

> Learn syntax → functions → OOP → libraries → projects → DSA.

**FORMALIZE**

> `I intend to develop proficiency in Python programming.`

**CASUALIZE**

> `I want to get really good at Python.`

**STORYIFY**

> `It started with one simple goal: learning Python...`

**POETIFY**

> `One line, one loop, one function at a time, I learn the language of Python.`

**MIMIC**

> Provide a reference text and ask the model to reproduce its relevant style or structure.

---

## 5. Creativity and Idea Generation Prompts

These techniques are useful when you want to **generate, transform, reverse, or challenge ideas**.

| Technique | Description | Example |
|---|---|---|
| **REMIX** | Take an existing idea and **recombine or modify it into a new version**. | `Remix a food-delivery app into a student-focused product.` |
| **REVERSE** | Flip the usual assumption, direction, or approach and explore the **opposite idea**. | `Reverse the concept of a traditional classroom.` |
| **BRAINSTORM** | Generate **many possible ideas** before filtering or judging them. | `Brainstorm 20 AI startup ideas for students.` |
| **DEVIL'S ADVOCATE** | Deliberately challenge an idea by identifying **weaknesses, objections, failure modes, or reasons it may not work**. | `Play devil's advocate on my startup idea.` |

### How they differ

- **BRAINSTORM** → Expand possibilities
- **REMIX** → Transform an existing idea
- **REVERSE** → Flip the assumption
- **DEVIL'S ADVOCATE** → Attack/test the idea

---

# 6. Image-Creation / Visual Output Shortcuts

These shortcuts are useful for asking an image-capable AI system to turn information into a particular **visual format**. They are best treated as **prompt vocabulary / workflow shortcuts**, not universal or official prompt-engineering commands.

| Shortcut | Status | Purpose | Example |
|---|---|---|---|
| **@Create image + /cheat sheet** | ✅ Added | Turn information into a compact **visual cheat sheet/reference card**. | `@Create image /cheat sheet: Python list methods, syntax, and examples.` |
| **@Create image + /blueprint** | ✅ Added | Turn a topic into a **structured visual blueprint/infographic** with hierarchy and sections. | `@Create image /blueprint: How a REST API works from client to database.` |
| **@Create image + \\blackchards** | ⚠️ Added as written | Visual shortcut mentioned in your session. **“blackchards” could not be verified as a standard term**, so confirm the spelling/meaning used by your instructor. | `@Create image \\blackchards: Explain the OSI model.` |
| **@Create image + /mindmap** | ✅ Added | Represent a topic as a **mind map**, with a central concept and connected branches. | `@Create image /mindmap: Machine Learning fundamentals.` |

### Important distinction

`@Create image` is the **image-generation instruction**. Terms such as `/blueprint` and `/mindmap` describe the **visual structure or format** you want. Current prompting resources document `/blueprint` used together with `@Create image`, and `/mindmap` is also used as a visual-format shortcut. citeturn941860search0turn941860search4

Do not treat every slash word as a hidden ChatGPT command. Some are simply shorthand that helps communicate the desired output format. A recent 2026 reference explicitly describes these kinds of “cheat codes” as prompt vocabulary/community shorthand rather than secret functionality. citeturn686744search5

---

# 7. Combining Techniques

The real power comes from **combining multiple prompting techniques**.

### Example

Instead of:

```text
Explain APIs.
```

Use:

```text
Act as a backend engineer teaching a 3rd-year CSE student.

Explain REST APIs.
Break the explanation down into 4 parts.
Use a real-world analogy.
Keep the language simple.
Give the final answer in 3 bullets.
End with the essence in 1 line.
```

This combines:

- **Role-based**
- **Breakdown**
- **Analogy**
- **Simplify**
- **3 bullets**
- **Essence**
- **1-liner**

---

# 8. Creative Workflow

A useful workflow for idea generation is:

```text
BRAINSTORM
     ↓
REMIX
     ↓
REVERSE
     ↓
DEVIL'S ADVOCATE
     ↓
REFINE
```

### Example

Idea:

> `Build an AI app that helps students study.`

**BRAINSTORM**

> Generate 20 possible implementations.

**REMIX**

> Combine the idea with gaming mechanics.

**REVERSE**

> Instead of helping students study more, design a system that helps them achieve the same learning outcome in less study time.

**DEVIL'S ADVOCATE**

> Identify the strongest reasons students may not use this product.

**REFINE**

> Improve the concept based on the identified weaknesses.

---

# 9. Example of a Full Multi-Technique Prompt

```text
Act as an experienced AI mentor.

I am a beginner learning Generative AI.

Explain Retrieval-Augmented Generation (RAG).

1. Break it down into simple components.
2. ELI10 the core idea.
3. Use a real-world analogy.
4. Give one practical example.
5. Explain the technical flow.
6. Condense the explanation into 3 bullets.
7. Give the essence in 1 line.
```

This is more precise because it specifies:

**WHO** → role  
**WHAT** → task  
**HOW** → explanation style  
**STRUCTURE** → output format  
**DEPTH** → desired level of detail

---

# 10. Ultra-Quick Cheat Sheet

```text
ZERO-SHOT       → No example
ONE-SHOT        → One example
FEW-SHOT        → Multiple examples
ROLE-BASED      → Assign a role

ELI5            → Very simple explanation
ELI10           → Simple, slightly deeper explanation
BREAKDOWN       → Split into parts
DEMYSTIFY       → Remove confusion
SIMPLIFY        → Make easier
ANALOGY         → Explain through comparison
VISUALIZE       → Help me picture it
T-TR            → Think → Translate → Respond*

ABSTRACT        → High-level summary
CONDENSE        → Shorter version
ESSENCE         → Core idea
1-LINER         → One sentence
3 BULLETS       → Three key points

PLANIFY         → Turn into a plan
FORMALIZE       → Make professional
CASUALIZE       → Make conversational
STORYIFY        → Turn into a story
POETIFY         → Make poetic
MIMIC           → Follow a reference style/pattern

REMIX           → Transform/recombine
REVERSE         → Flip the usual approach
BRAINSTORM      → Generate many ideas
DEVIL'S ADVOCATE→ Challenge the idea

IMAGE / VISUAL SHORTCUTS
@CREATE IMAGE /CHEAT SHEET → Visual reference/cheat sheet
@CREATE IMAGE /BLUEPRINT   → Structured visual blueprint
@CREATE IMAGE \\BLACKCHARDS → Session-specific term; verify spelling/meaning*
@CREATE IMAGE /MINDMAP    → Visual mind map
```

> `* T-TR is included as it was discussed in your session; confirm your instructor's exact definition because it is not a universally standardized prompting term.`

> `** The README preserves “blackchards” exactly as you wrote it. I could not verify it as a standard prompting term; check whether your instructor meant a different spelling.`

---

## 11. The Core Idea

Prompt engineering is largely about controlling four things:

```text
CONTEXT       → What the model should know
TASK          → What the model should do
STYLE         → How it should respond
OUTPUT        → What the final result should look like
```

A strong prompt does not need every technique. Use only the ones that improve the result.

### A simple formula

```text
ROLE + CONTEXT + TASK + CONSTRAINTS + OUTPUT FORMAT
```

Example:

```text
Role: Act as a Python tutor.
Context: I am a beginner.
Task: Explain decorators.
Constraints: Avoid jargon.
Output: Use an analogy + 3 bullets + 1-line essence.
```

---

## License

This cheat sheet is a personal learning reference and can be freely adapted for notes, study, or project documentation.
