# Milan Khati

Backend and AI engineer in Kathmandu, Nepal. Open to relocation.

I build backend services and the LLM features that sit on them: document
extraction, RAG, and agent workflows, plus the queues, billing, and APIs
around them. The projects below are products I built and run myself.

## Projects

### OCRQueen: document extraction API

[ocrqueen.com](https://ocrqueen.com) · App source is private, SDKs and API spec are public

Turns PDFs, slides, and images into structured JSON and Markdown.

- Async FastAPI API with arq workers.
- Docling reads the page layout, then an LLM extracts each page into a Pydantic schema.
- If one model provider fails on a page, the next one is tried, so one bad page does not fail the document.
- Prepaid billing that stays correct when jobs run at the same time: funds are reserved first and settled on the real page count.
- Signed webhooks with retries, and idempotency keys against duplicate work.
- SDKs for [Python](https://github.com/iammilankhati/ocrqueen-python) ([PyPI](https://pypi.org/project/ocrqueen/)) and [Node](https://github.com/iammilankhati/ocrqueen-node) ([npm](https://www.npmjs.com/package/ocrqueen)), built from one [OpenAPI spec](https://github.com/iammilankhati/ocrqueen-openapi).

### SikshyaLab: learning platform with live classes

[sikshyalab.com](https://sikshyalab.com) · Source is private

A multi-tenant platform for schools and tuition centres: courses, live
classes, exams, attendance, and AI study tools.

- NestJS API, a FastAPI and LangGraph service for the AI features, and a Next.js app, on PostgreSQL.
- Turns a teacher's own material into quizzes, exams, flashcards, and notes, and answers student questions from the same content.
- Live classes run on self-hosted LiveKit. I measured CPU use per student and per recording on real classes, and sized the servers from those numbers.
- Each school's limit on classes running at once is enforced with PostgreSQL locks.

### Pipeero: forms, databases, and questions in plain language

[pipeero.com](https://pipeero.com) · Source is private

Teams collect data through forms and uploaded documents, connect their
own MySQL, PostgreSQL, or MongoDB database, and ask questions about it in
a chat.

- Questions about totals are answered by SQL over the full data. The model decides what to compute and explains the result. It does not do the arithmetic.
- Search over submissions and documents with pgvector.
- Signed outgoing webhooks, queued on BullMQ with retries.

### AI support-agent platform (in progress)

[ai-support-agent-platform](https://github.com/iammilankhati/ai-support-agent-platform)

Agents that resolve support tickets by calling tools, on Kafka, Redis,
and PostgreSQL. Requirements and design are written. The build is in
progress.

## What I work with most

Python (FastAPI, Django) · TypeScript (NestJS, Next.js) · PostgreSQL ·
Redis · LangGraph · pgvector · AWS · Docker

## Contact

[LinkedIn](https://www.linkedin.com/in/milan-khati/)
