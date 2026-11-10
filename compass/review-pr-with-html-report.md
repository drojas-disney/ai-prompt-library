`{{pr_url}}`

Review this pull request using your normal workflow, including adding PR comments where appropriate.

In addition, generate a **self-contained HTML report rendered directly in this chat window** that explains the technical implementation of the PR.

## HTML Report Requirements

The report is intended to help a developer understand exactly what changed, how it works, and how it affects the application.

Include the following sections:

### 1. Summary
- What the PR accomplishes and why.
- The functionality being added, modified, or removed.
- A high-level explanation of the implementation approach.

### 2. Architecture & Execution Flow
- Explain how the changes fit into the existing architecture.
- Describe the execution flow, including how the affected components interact.
- Explain relevant programming concepts, patterns, and design decisions.
- Include diagrams where they improve understanding.

### 3. Code Changes
Provide a detailed, file-by-file explanation of the meaningful changes.

- Include relevant code snippets from the PR.
- Explain what each change does and why it is necessary.
- Describe how new or modified classes, methods, interfaces, and dependencies work together.
- Explain technical details rather than simply repeating or summarizing the diff.
- Use before/after comparisons where helpful.
- Include sufficient surrounding code to make each snippet understandable.

### 4. Affected APIs & Endpoints
If applicable:
- Identify endpoints added, modified, or removed.
- Include HTTP methods, paths, and relevant request/response structures.
- Explain how requests are processed and which components are involved.
- Describe changes in behavior, data flow, and interactions with downstream services.
- Distinguish externally observable behavior changes from internal implementation changes.

## Report Format & Visual Design

- Render the HTML report **directly in this chat window**. Do not attempt to create or attach a downloadable file.
- Use a clean, modern, responsive layout with horizontal tab navigation for the report sections.
- Make the report easy to navigate, with clear headings, consistent spacing, tables where appropriate, and visually distinct code blocks.
- Use embedded CSS and JavaScript where supported, without requiring external resources.
- Include syntax-highlighted code snippets with file paths and relevant line references.

### Code Readability & Color Contrast

**Code readability is a strict requirement.**

- Ensure strong contrast between text and background in every code block, including inline code, syntax-highlighted snippets, and before/after comparisons.
- Never render dark text on a dark background or light text on a light background.
- Prefer a dark code-editor theme with a near-black background and bright, clearly distinguishable syntax colors.
- Use an explicit foreground color for all code text, including tokens without syntax highlighting.
- Ensure syntax highlighting does not override readability. Avoid dark blue, dark purple, or similarly low-contrast colors against dark backgrounds.
- Use a monospace font with comfortable font size, line height, and indentation.
- Preserve source-code formatting, indentation, and line breaks.
- Allow horizontal scrolling for long lines rather than clipping code.
- Ensure code remains readable regardless of whether the surrounding chat interface uses light or dark mode.
- Aim for at least a 4.5:1 contrast ratio for normal text, including syntax-highlighted tokens.
- If reliable syntax highlighting is unavailable, use uniformly light-colored code text on a dark background rather than potentially unreadable highlighting.

## Accuracy & Technical Depth

- Base all explanations on the actual PR changes and relevant repository context.
- Do not invent implementation details, endpoint behavior, or architectural relationships.
- Clearly distinguish verified behavior from assumptions.
- Explain the reasoning behind implementation decisions when it can be established from the code.
- Prioritize technical depth and clarity over brevity.
- Do not merely paraphrase the diff. Explain the actual runtime behavior and how the changed components interact.

## Important Constraints

- **Continue your normal PR review workflow independently of this report.**
- **Exclude tests and test-related changes from the HTML report.**
- Focus the HTML report on technical explanation, not code-review findings or recommendations.
- Do not post, attach, link, or mention the HTML report in the PR or its comments.
- Do not commit the report to the repository.
- The HTML report is exclusively for this chat conversation.
- Render the completed report directly in the chat using the available HTML rendering capabilities.
