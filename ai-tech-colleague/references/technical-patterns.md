# Technical Patterns

Use this only when the user needs help understanding what technology might be involved. Keep explanations beginner-friendly.

## Plain-Language Map

| User Need | Simple Capability | How To Explain It |
| --- | --- | --- |
| Answer questions from company documents | Knowledge Q&A / RAG | "先找相关资料，再让 AI 根据资料回答。" |
| Find similar documents or meanings | Semantic search / Embedding | "不只搜关键词，而是按意思找。" |
| Read scanned files, invoices, forms | OCR | "先把图片里的字识别出来。" |
| Pull fields from text | Structured extraction | "把一段话变成固定字段，比如金额、日期、负责人。" |
| Write weekly reports or replies | Draft generation | "AI 先写草稿，人再改。" |
| Sort tickets or emails | Classification | "把内容分到几个固定类别里。" |
| Explain business numbers | Data system + AI explanation | "数据系统算数字，AI 负责翻译成人话。" |
| Handle a fixed process | Workflow + AI step | "流程照旧，AI 只帮其中一小步。" |
| Let AI choose tools by itself | Agent | "AI 自己决定下一步做什么，第一版要谨慎。" |

## Simple Choice Rules

- If the answer must come from documents, use **knowledge Q&A**.
- If the task is reading invoices, contracts, screenshots, or scanned forms, use **OCR + extraction**.
- If the task is generating reports, emails, or summaries, use **draft generation**.
- If the task is assigning category, urgency, owner, or type, use **classification**.
- If the task is about numbers, let **BI/database calculate** and let AI explain.
- If the process is fixed, use **workflow**, not a free agent.
- If someone asks for an **Agent**, first ask: "Does AI really need to decide the next step, or is the process actually fixed?"

## Terms To Avoid Unless Needed

Avoid leading with these terms for beginner users:

- Vector database
- Semantic layer
- Reranking
- Orchestration
- Observability
- Fine-tuning
- Agentic workflow

If you must mention them, add one plain sentence explaining what they mean.
