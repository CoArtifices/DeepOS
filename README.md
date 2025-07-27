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

## 🛠️ DeepOS Architecture

**DeepOS** operates under a modular **agent-based design**, with a **Large Language Model (LLM)** at its core orchestrating interactions.

```
+---------------------+      +------------------------+
|   User (CLI/Web)    | <--> |     UI Module          |
+---------------------+      +------------------------+
           |                             ^
           v                             |
+---------------------+                  |
| Input Preprocessor  |                  |
+---------------------+                  |
           |                             |
           v                             |
+---------------------+                  |  (Responses,
|  Central Agent (LLM)| <-----------------+   App State)
|    (Orchestrator)   |                  |
+---------------------+                  |
    |  ^   ^   ^                         |
    |  |   |   |                         |
    v  |   |   |                         v
+----------+----------+      +-----------------------+
|   App Parser        |      |  App State Manager    |
| (Interprets Documents)|    |  (App's Memory)       |
+-----------------------+      +-----------------------+
    |                                   ^
    v                                   |
+-----------------------+               |
|  Execution Engine     | <-------------+
|   (Secure Sandbox)    |
+-----------------------+
    |
    v
+-----------------------+
|   System APIs         |
| (Generic Functions)   |
+-----------------------+
```

  * **UI Module:** The interaction point with the user (conversational command line or web interface).
  * **Input Preprocessor:** Cleans and prepares user input, manages conversation context.
  * **Central Agent (LLM):** The "brain" of **DeepOS**. It interprets intent, plans actions, and orchestrates calls to other modules. This is where the base LLM (e.g., Llama 3, Mistral) resides.
  * **App Parser:** Reads and comprehends the structure and logic of "apps" defined in text documents.
  * **App State Manager:** Maintains and updates the internal state of the running application (e.g., AInopoly board, calculator variables).
  * **Execution Engine (Sandbox):** Securely executes the logical instructions extracted by the LLM from the app document, interacting with the App State Manager.
  * **System APIs:** A set of abstract, generic functions (e.g., `transfer_value`, `set_variable`) that the Execution Engine can invoke at the app's request.

-----

## 🗺️ Roadmap (Next Steps)

Our journey is ambitious, and we're seeking collaboration to:

  * **Expand System APIs:** Add more generic functions for complex operations (list management, random number generation, date handling, etc.).
  * **Enhance Rule Language:** Develop a more robust and flexible DSL (Domain-Specific Language) for writing apps in documents, allowing for more intricate logic and complex data patterns.
  * **State Persistence:** Enable apps to save and load their state across sessions, crucial for long-running games or management tools.
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
