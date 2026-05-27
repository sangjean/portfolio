# 🚀 1-Page Portfolio Website Development Project Specification (AGENTS.md)

This document (AGENTS.md) serves as the development guidelines and architectural blueprint for a single-page (`index.html`) dark-theme portfolio website, showcasing the core project capabilities and technical stack of **Kim Sang-jin**, a Computer Science and Engineering major.

---

## 1. Project Overview

* [cite_start]**Developer:** Kim Sang-jin (Student ID: 2022136020) [cite: 1]
* **Project Name:** 1-Page Dark-Theme Developer Portfolio
* **Objective:** To build a single-page portfolio that intuitively demonstrates core competencies in visualizing complex system mechanisms and designing dynamic web architectures.
* **Core Design Identity:**
    * **Dark Mode Theme:** Utilizing a deep, dark background palette (`#0f172a`, `#1e293b`) paired with sophisticated accents (Slate Blue / Orange Accent) to create a modern, immersive UI tailored for a software engineer.
    * **Single-File Compactness:** Heavily integrating the structure (HTML), styling (CSS), and logic (JS) into a single `index.html` file to maximize initial loading speed.
* **Tech Stack:** HTML5 (Semantic Web), CSS3 (Flexbox/Grid, Custom Properties), JavaScript (Vanilla ES6+)

---

## 2. Website Structure & Content Blueprint

The portfolio website flows sequentially through four core sections within a single-page layout.

### 2.1 Navigation Bar
* **Menu Items:** `Home` | `About Me` | `Projects` | `Contact`
* [cite_start]**Behavior:** Smoothly glides to the target section upon clicking (`scroll-behavior: smooth;`). 

### 2.2 Hero Section (Main Screen)
* [cite_start]**Main Title:** "A developer who creates value by visualizing mechanisms beyond theory, I am Kim Sang-jin." [cite: 118]
* **Sub-copy:** Hello! [cite_start]I am a computer science student who finds passion in implementing and visualizing complex system mechanisms and dynamic web architectures[cite: 1, 118, 133]. [cite_start]I aim to build robust software that thoroughly handles edge cases and protects against user exceptions[cite: 126]. [cite_start]When faced with intricate bugs, I am dedicated to analyzing and researching deep into the problem to find a clean, efficient solution[cite: 124, 126].

### 2.3 About Me & Skills Section
* **Technical Stack Categorization:**
    * [cite_start]**Languages:** C++, PHP, JavaScript (ES6+), HTML5/CSS3 [cite: 1, 133, 146]
    * [cite_start]**Frameworks & Tools:** MFC, Apache (XAMPP/WampServer environment) [cite: 1, 143]
    * [cite_start]**Database:** MySQL (Relational Database Design) [cite: 133, 143]
    * [cite_start]**Core CS:** Operating Systems (Semaphore synchronization, Mutual Exclusion process control) [cite: 1, 118]

### 2.4 Projects Section (2 Core Projects)
1. [cite_start]**⚾ Dynamic Interaction-Based 'Hanwha Eagles Fan Page'** [cite: 133]
    * [cite_start]*Tech Stack:* PHP, MySQL, Apache, HTML5/CSS3, JavaScript [cite: 133, 143, 146]
    * [cite_start]*Key Implementations:* Built a scheduler that automatically updates match schedules based on the current date[cite: 161, 163]. [cite_start]Implemented dynamic roster filtering using GET method query strings[cite: 179, 180]. [cite_start]Solved the integer-bound truncation issue for '00-numbered' developmental players by applying a data manipulation algorithm with `sprintf` string formatting[cite: 190, 191]. [cite_start]Developed a secure fan community platform utilizing `INNER JOIN` operations and robust session validation for access control and author-specific deletion capabilities[cite: 213, 214, 229].
2. [cite_start]**🔄 Producer-Consumer Problem Simulator Using Circular Multi-Buffers** [cite: 1, 2]
    * [cite_start]*Tech Stack:* C++, MFC (Microsoft Foundation Class) [cite: 1]
    * [cite_start]*Key Implementations:* Created a text-based scenario parsing engine that processes P (Producer) and C (Consumer) commands separated by commas from a `scenario.txt` file[cite: 4]. [cite_start]Designed a real-time graphical status dashboard mapping buffer data presence (0 or 1), pointer indexes (`in`/`out`), and semaphore counters (`nrfull`/`nrempty`)[cite: 6, 7, 8]. [cite_start]Visualized the active waiting queues for blocked processes and debugged complex cross-class rendering synchronization and timing issues[cite: 9, 121, 122].

### 2.5 Contact Section
* **Information Displayed:** Placeholders for Email Address, GitHub Repository Link, and Tech Blog URL.

---

## 3. Project Architecture Diagram

```text
       [ User Browser ]
               │
               ▼
   ┌──────────────────────┐
   │      index.html      │ (Built-in Dark Theme)
   └───────────┬──────────┘
               │
      ┌────────┼────────┐
      ▼        ▼        ▼
┌──────────┐┌──────────┐┌──────────────┐
│Structure ││ Styling  ││ Interaction  │
│ (HTML5)  ││  (CSS3)  ││  (JS ES6+)   │
├──────────┤├──────────┤├──────────────┤
│- Header  ││- Dark    ││- Smooth      │
│  & Nav   ││  Palette ││  Scrolling   │
│- Hero    ││  (#0f172a)││- Intersection│
│  Section ││- Custom  ││  Observer    │
│- Skills  ││  Vars    ││- Active Link │
│- Projects││- Flex/Grid││  Highlight   │
│- Contact ││- Respon- ││              │
│  Form    ││  sive    ││              │
└──────────┘└──────────┘└──────────────┘
               │
               ▼
   ┌──────────────────────┐
   │   Assets & Images    │
   │ (WebP Project Cards) │
   └──────────────────────┘