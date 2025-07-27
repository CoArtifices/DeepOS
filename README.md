# DeepOS
An experimental AI-powered operating system in which executable programs are documents written in natural language.

-----


## 🚀 Unlock the Potential of Conversational Apps

**DeepOS** is an experimental open-source operating system that redefines how we interact with software. Forget complex programming languages; with DeepOS, your **applications are written and executed directly from natural language text documents**.

Imagine a future where a spreadsheet, a board game, or a project management tool comes to life by simply pasting its rules and logic into a document. **DeepOS** is the **core** that makes this possible, interpreting your human language instructions and transforming them into executable actions.

-----

## ✨ Our Vision: Documents as Programs

Traditional operating systems execute binary code. DeepOS elevates abstraction, allowing **human language to be the programming interface**. Our goal is to build an application-agnostic platform that provides the resources and infrastructure for any "app" defined in a text document to run smoothly and conversationally.

DeepOS's core doesn't inherently "know" the rules of a specific game or the logic of a productivity tool. Instead, it acts as an **intelligent orchestrator** that:

  * **Interprets:** Understands the logic and rules defined in your app documents.
  * **Manages Resources:** Provides an environment for apps to store and manipulate their state (like virtual memory for app data).
  * **Executes Actions:** Translates app instructions into calls to a set of abstract, secure system APIs.

This means the **application's complexity resides entirely within the document**, not in the DeepOS codebase. Want to change a game rule? Edit the document. Want to create a new app? Write a new document.

-----

## 🛠️ DeepOS Architecture: How It Works

**DeepOS** operates under a modular **agent-based design**, with a **Large Language Model (LLM)** at its core orchestrating interactions.

```
+---------------------+           +--------------------------+
|      USER           |           |   1. INTERFACE MODULE    |
| (CLI / Web UI)      | <-------> | (Handles User Input/Output)|
+---------------------+           +--------------------------+
           |                                  ^
           | User Query / Commands            | DeepOS Responses / App Output
           v                                  |
+-----------------------------------------------------------+
|               2. DEEPOS CORE (The "Brain")                |
|               (Powered by an LLM Agent)                   |
|                                                           |
|  - **Interprets Intent:** Understands user commands and    |
|    app logic from documents.                              |
|  - **Orchestrates Actions:** Decides what needs to be done |
|    and which modules/tools to use.                        |
|                                                           |
+-----------------------------------------------------------+
    |           ^           ^           ^
    |           |           |           |
    v           |           |           |
+-----------------+   +-----------------+   +-----------------+
| 3. APP PARSER   |   | 4. APP STATE    |   | 5. EXECUTION    |
| (Reads App      |   | MANAGER         |   | ENGINE          |
|  Documents &    |   | (Manages App    |   | (Runs App Logic |
|  Extracts Logic)|   | Data/Memory)    |   | in a Sandbox)   |
+-----------------+   +-----------------+   +-----------------+
        |                   ^                       |
        | App Logic/Rules   | App Data/State        | Abstract Actions/APIs
        v                   |                       v
+-----------------------------------------------------------+
|              6. SYSTEM APIs (DeepOS Capabilities)         |
|              (Generic functions for apps to use)          |
+-----------------------------------------------------------+
```

  * **1. Interface Module:** This is where you interact with DeepOS. It takes your commands and questions and displays DeepOS's responses or the output from your running apps.
  * **2. DeepOS Core (The "Brain"):** Powered by a Large Language Model (LLM), this is the central intelligence. It understands what you want to do (whether it's a system command or an app instruction), plans the necessary steps, and directs other modules to perform tasks.
  * **3. App Parser:** When you load an app, this module reads its document. It extracts the rules, logic, and data (like a game's board or a table's structure) written in natural language, translating them into a format DeepOS can work with.
  * **4. App State Manager:** This module is the "memory" for your apps. It keeps track of all the app's current data – for AInopoly, that would be player money, property ownership, board positions, etc. – and updates it as the app runs.
  * **5. Execution Engine:** This is the "CPU" for your apps. It securely runs the specific logic and instructions provided by the app document. It takes input from the App Parser and uses the App State Manager to perform actions.
  * **6. System APIs (DeepOS Capabilities):** These are the fundamental, generic tools DeepOS provides to all apps. Think of them as basic building blocks like "transfer value," "set variable," or "get data." The Execution Engine uses these to carry out the app's instructions.

-----

## 🚀 Get Started: Your First App on DeepOS

The goal of **DeepOS** is to demonstrate the ability to run simple apps from documents.

### **Current Features:**

  * **Document-App Loading:** DeepOS can load and process text files (Markdown recommended) containing application logic.
  * **"Hello World" Execution:** A functional example of an app that simply greets the user, defined within a document.
  * **Simple Calculator:** An app defined in a document that can perform basic operations (like addition) based on natural language instructions.

-----

## 🗺️ Roadmap (Next Steps)

Our journey is ambitious, and we're seeking collaboration to:

  * **Expand System APIs:** Add more generic functions for complex operations (list management, random number generation, date handling, etc.).
  * **Enhance Rule Language:** Develop a more robust and flexible DSL (Domain-Specific Language) for writing apps in documents, allowing for more intricate logic and complex data patterns.
  * **State Persistence:** Enable apps to save and load their state across sessions, which is crucial for long-running games or management tools.
  * **Complex App Support:** Enable the execution of more sophisticated applications. This could include:
      * **A simple task manager:** With rules for adding, completing, and prioritizing tasks.
      * **A basic inventory management system:** Where the document defines items, their quantities, and rules for adding/deducting stock.
      * **An interactive table assistant:** A kind of **basic Excel** where the app document defines the initial table structure, cell operation rules (e.g., "column C is the sum of A and B"), and conditions for data manipulation. DeepOS users could then query, summarize, or perform analysis on the table data using the OS's AI capabilities.
      * Our flagship implementation: a reduced version of **AInopoly**. In this case, the game will come to life based on the **set of rules, board data, card descriptions, and game contexts** entirely specified within the application document.
  * **Web Interface:** Develop a more user-friendly web-based interface for smoother interaction.

-----

## 🤝 How Can You Contribute?

**DeepOS** is an open-source project, and your help is invaluable\! We're looking for curious and passionate minds in:

  * **Machine Learning / NLP Engineering:** LLM fine-tuning, prompt design, agent reasoning.
  * **Software Engineering:** Module development (parser, execution engine, state management), API design.
  * **Systems Design:** Architecture, scalability, security.
  * **Language Design:** Creating our natural language-based "rule language."
  * **Documentation and Testing:** Writing examples, guides, and ensuring code quality.

Please see our [`CONTRIBUTING.md`](https://www.google.com/search?q=CONTRIBUTING.md) file for more details on how to get started. Join us in building the future of human-computer interaction\!

-----

**Be part of the natural language revolution\!**
