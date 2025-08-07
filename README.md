# Document_comparator
Put in two pdf documents and compare them 

<img width="1905" height="958" alt="Screenshot from 2025-08-07 22-30-31" src="https://github.com/user-attachments/assets/542747cb-a4a0-479b-93e3-915e5de1a4b1" />


🤖 AI-Powered Document Comparator

An intelligent tool that uses an OpenAI Agent-based workflow to perform a deep, contextual comparison of two documents. Upload your files (PDF, DOCX, or TXT) and receive a detailed analysis covering summaries, similarities, and differences.

🌟 About The Project

Traditional document comparison tools often rely on simple text-matching (diff algorithms), which can miss contextual nuances, thematic similarities, or high-level conceptual differences. This project takes a modern approach by leveraging an AI agentic workflow to analyze and compare documents like a human expert would.

The system first understands the core content of each document and then performs a structured comparison, providing insights that go beyond word-for-word changes.

✨ Features

    Multi-Format Support: Upload and compare .pdf, .docx, and .txt files.

    AI-Generated Summaries: Get a quick, high-level summary of each document to understand its purpose and content at a glance.

    Contextual Comparison: The AI agent identifies and lists key similarities and differences, focusing on themes, arguments, and structure.

    Structured Output: The final report is clearly organized into sections for easy reading and analysis.

    Simple Web Interface: Built with Gradio for a clean, user-friendly experience.

🧠 How It Works: An Agentic Workflow

This project's intelligence comes from a multi-step, agent-based process orchestrated in Python:

    Document Ingestion: The user uploads two documents through the Gradio frontend. The Python backend uses libraries like pypdf and python-docx to extract the text content.

    Agent Tasking: An OpenAI Agent (or Assistant) is tasked with a multi-step goal:

        Step 1: Summarize. The agent first reads Document A and Document B independently to generate a concise summary for each. This establishes a foundational understanding.

        Step 2: Compare. The agent then analyzes both documents (or their summaries) to identify points of convergence and divergence. It looks for common themes, shared terminology, and structural parallels to find similarities. It also identifies conflicting information, different scopes, or unique points to find differences.

    Report Generation: The agent compiles its findings into a single, structured Markdown report.

    Display: The final report is sent back to the Gradio interface and displayed to the user.

This agentic approach allows the system to perform complex reasoning tasks, resulting in a much more insightful comparison than simple algorithms.

🛠️ Tech Stack

    Backend: Python

    AI Engine: OpenAI API (Assistants/Agents)

    Web UI: Gradio

    Document Parsing: PyPDF2, python-docx
