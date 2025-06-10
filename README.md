# Multi-Agent AI Content Researcher (CrewAI + HuggingFace)

This repository demonstrates a multi-agent system using [CrewAI](https://docs.crewai.com/) and `huggingface` to simulate a team of AI agents that collaboratively plan, write, and edit insightful blog content on any given topic.

## Project Purpose

This project is a sandbox for building and testing **autonomous agents** that act as a **researcher, writer, and editor**, working together to create factually accurate, SEO-optimized, and professionally written blog posts.


##  Agent Architecture

The system includes **three specialized agents**, each with a distinct role in the content generation pipeline:

###  1. Content Planner
- **Goal:** Plan engaging and factually accurate content on `{topic}`.
- **Backstory:** Research trends, analyze the target audience, and create a content plan that serves as the foundation for the writer.
- **Tasks:**
  - Identify audience pain points.
  - Prioritize latest news and trends.
  - Generate outline and SEO keywords.

### 2. Content Writer
- **Goal:** Write a compelling blog post based on the planner’s outline.
- **Backstory:** Produces insightful and well-structured writing that respects factual context while acknowledging opinions.
- **Tasks:**
  - Craft content with intro/body/conclusion.
  - Use SEO naturally and follow brand voice.
  - Maintain clarity and readability.

### 3. Editor
- **Goal:** Finalize the blog post for publication.
- **Backstory:** Reviews grammar, tone, and alignment with editorial guidelines while avoiding polarizing or controversial statements.
- **Tasks:**
  - Proofread and polish.
  - Ensure balanced and brand-aligned writing.


## Task Flow

| Step | Agent | Task |
|------|-------|------|
| 1️ | **Content Planner** | Create a comprehensive content plan with an outline, audience profile, SEO keywords, and references. |
| 2️ | **Content Writer** | Write the full blog post using the planner's output. Structure it in Markdown with 2–3 paragraphs per section. |
| 3️ | **Editor** | Edit and proofread the article, ensuring clarity, brand tone, and journalistic best practices. |
