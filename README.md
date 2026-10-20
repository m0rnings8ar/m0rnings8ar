# Ashutosh Jha

## 🚀 About Me
Hello! I'm Ashutosh Jha, a full-stack engineer and Senior Software Engineer at InfoEdge (99acres). I build products end to end, from NestJS services, REST APIs, and Redis caching that handle ~35K requests/min to React and React Native apps used every day. Most recently I built XID, an AI-assisted platform where Gemini-powered extraction, a decisioning engine, and a mobile review app cut Ops request handling from ~30 minutes to ~5. Previously at Skuad (acquired by Payoneer), I shipped full-stack features for a global payroll platform, from the Time Off module to the Resume Builder. I enjoy owning a feature from the first conversation with users through to production.

## 💼 Work Experience

### Senior Software Engineer at InfoEdge (99acres)
*Jan 2025 - Present*
- Built XID, an AI-assisted Ops platform, end to end (NestJS backend services and React Native app), turning Sales and RERA requests (300-400+ RERA requests/week) into project and tower changes and cutting per-request handling for ~150 Ops personnel from ~30 min of manual entry to ~5 min of review.
- Designed XID's decisioning engine and create/update REST APIs: ranking sources by priority, resolving conflicting values with field-level rules, and owning validation, persistence, and failure paths.
- Migrated document extraction from LandingAI to Gemini Flash with schema-constrained structured outputs, validating every model-derived value before any mutation.
- Built the XID mobile app in React Native and Redux with resumable multi-step submissions, retryable document uploads, and review screens that flag AI-extracted values and cross-source conflicts for Ops to confirm.
- Added a Redis cache-aside layer to the core project data service (~35K requests/min), with the hottest endpoint at 11 ms average latency, and built aggregator APIs for the project detail, search, and media pages at 300-400 ms p95.
- Made submissions idempotent across the stack (in-flight UI guards plus backend idempotency keys), holding average latency under 150 ms through traffic spikes, monitored with Elastic APM.

### Software Engineer at Skuad (Acquired by Payoneer)
*Jul 2022 - Dec 2024*
- Built the Time Off module end to end (React/Redux UI, NestJS/MongoDB APIs): leave requests, country holiday calendars, leave balances, and manager approvals for a global workforce.
- Fixed leave dates shifting by a day across time zones by storing them as date-only values and applying each country's holiday calendar to leave counts.
- Built production services in Node.js, TypeScript, and NestJS on MongoDB and Redis, including event-driven workflows on Kafka and RabbitMQ with retries and error handling.
- Developed REST and GraphQL APIs with validation and business rules, wrote API and integration tests, and shipped through Docker and GitHub Actions CI/CD on Google Cloud.
- Contributed to a 40% reduction in production defects by debugging live issues across APIs, queues, and databases and improving monitoring and validation coverage.

### Software Engineer (Intern) at Skuad
*May 2022 - Jun 2022*
- Owned the Resume Builder ([allremote.jobs/resume](https://allremote.jobs/resume)) end to end: Next.js (SSR) and Redux frontend, Node.js/NestJS APIs, and template-based PDF export.
- Fixed live-preview lag on long resumes by debouncing form input and memoizing each template section so only the edited section re-rendered.
- Made exported PDFs match the on-screen preview by rendering both from the same HTML templates and print CSS; converted to full-time in July 2022.

### Web Developer at BlueHelmet
*September 2021 - November 2021*
- Designed and launched a customer-centric website and a job seeker platform utilizing ReactJS, enhancing user engagement and functionality.
- Seamlessly integrated Servetel SMS API and configured a PostgreSQL database for local server testing, optimizing system performance and reliability.

## 🌟 Projects

- **[AI Gateway Platform](https://ai-utility-suite.vercel.app)**: Built a full-stack AI gateway for chat, summarization, translation, and information extraction with authentication, rate limiting, streaming responses rendered incrementally, usage/cost tracking, and validation and failure handling around every model call. [Source Code](https://github.com/m0rnings8ar/ai-utility-suite)

- **[AllRemote Jobs Website](https://allremote.jobs/)**: Remote-jobs platform by Skuad for discovering remote roles, building resumes, and joining hackathons. I owned its Resume Builder end to end: a Next.js (SSR) and Redux editor with debounced live preview, NestJS APIs, and template-based PDF export that matches the on-screen preview exactly.

- **[PoseNet Character Animation](https://github.com/m0rnings8ar/CharAnimation)**: In-browser character animation driven by real-time body-pose tracking with TensorFlow.js and PoseNet, mapping 17 body keypoints to an animated character at 30 FPS.

- **[Next.js ChatGPT Integration](https://github.com/Ashutoshjha001/ChatGptWithNextJs)**: Developed an advanced conversational AI application by integrating OpenAI's GPT-3 model into a Next.js framework. This project allows users to interact with an AI-powered chatbot capable of generating contextually relevant and coherent responses in real-time. The integration involves complex API handling, session management, and UI/UX design to create a seamless, user-friendly interface. This application can be adapted for customer service, virtual assistants, or any platform requiring natural language processing capabilities.

## 💪 Skills & Strengths

### Languages
- JavaScript, TypeScript, Java, Python, SQL

### Frontend
- React, Next.js (SSR), React Native, Redux, TailwindCSS, Styled-Components, NextAuth.js

### Backend
- Node.js, NestJS, Express.js, REST APIs, GraphQL, Kafka, RabbitMQ

### AI / LLM
- Gemini, OpenAI API, Structured Outputs, Schema Validation & Guardrails, Prompt Engineering

### Databases
- PostgreSQL, MongoDB, Redis, BigQuery, Firebase

### Tools & DevOps
- Git, GitHub, GitHub Actions, CI/CD, Docker, Google Cloud, Nginx, Postman, Elastic APM

### Core Strengths
- Full-Stack Product Engineering
- Backend & API Design
- React & React Native Apps
- AI / LLM Integration
- Caching & Performance
- Event-Driven Architecture
- Product-Driven Engineering
- Production Debugging & Observability
- Collaborative Mindset

## 🛠️ Running This Portfolio Locally

Built with Next.js, TailwindCSS, Framer Motion, and React Three Fiber. All portfolio content (experience, projects, skills, socials) lives in [`constants/index.js`](constants/index.js).

Requires **Node.js 24** (pinned in `.nvmrc` and `package.json` engines; run `nvm use` if you use nvm).

```bash
npm install
npm run dev     # http://localhost:3000
npm run build   # production build
```

### Contact form (EmailJS)
The contact form sends mail through [EmailJS](https://www.emailjs.com/) and needs these variables in a `.env.local` file at the project root (gitignored):

```
NEXT_PUBLIC_SERVICE_ID=service_xxxxx
NEXT_PUBLIC_TEMPLATE_ID=template_xxxxx
NEXT_PUBLIC_EMAILJS_KEY=your_public_key
```

Find them in the EmailJS dashboard under **Email Services**, **Email Templates**, and **Account → Public Key**. Restart the dev server after adding them. Without them the form shows "Submission Failed" and no request is sent.

On Vercel, add the same variables under **Project → Settings → Environment Variables** and redeploy, since `NEXT_PUBLIC_*` values are inlined at build time.

## 📫 Contact
- Email: [jhaashutosh9717@gmail.com](mailto:jhaashutosh9717@gmail.com)
- LinkedIn: [LinkedIn Profile](https://www.linkedin.com/in/m0rnings8ar/)
- GitHub: [GitHub Profile](https://github.com/m0rnings8ar)
- X (Twitter): [@m0rnings8ar](https://twitter.com/m0rnings8ar)
- Instagram: [@m0rnings8ar](https://www.instagram.com/m0rnings8ar/)

