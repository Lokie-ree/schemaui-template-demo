Okay, this PRD is structured specifically for using Cursor's `Ask` (understanding) and `Agent` (modification/prototyping) features on an ongoing basis. It frames the codebase not just as something to understand once, but as a foundational asset for future, niche client work, particularly related to AI advancements.

---

## Living PRD: Exploring & Adapting the [Sanity Schema UI Template Name] for Niche AI-Driven Solutions

**Version:** 1.0 (Living Document)
**Date:** 2023-10-27 (Last Updated: [Current Date])
**Status:** Ongoing Exploration & Adaptation
**Authors:** [Your Name/Team Name]
**Template Link:** [Link to Template Repo/Docs if available]

**1. Introduction**

*   **Purpose:** To continuously explore, understand, modify, and document the '[Sanity Schema UI Template Name]' codebase using **Cursor**. This PRD guides our use of **Cursor Ask** for deep comprehension and **Cursor Agent** for prototyping modifications and adaptations.
*   **Strategic Context:** This template serves as a potential foundation for rapidly developing custom Sanity Studio experiences for clients in **specific niches**, with a forward-looking focus on areas impacted by **AI advancements** (e.g., content generation workflows, data annotation, prompt management, AI model interaction UIs).
*   **Methodology:** We will iteratively use Cursor's AI capabilities:
    *   **Ask (`Cmd+K`, Chat):** To query the codebase, understand component logic, trace data flow, explain configurations, and identify customization patterns.
    *   **Agent (`Cmd+Enter`, Chat):** To prototype changes, refactor code, generate boilerplate for new schemas/components, and implement experimental UI adaptations based on our understanding and brainstorming.
*   **Goal:** To build a deep, actionable understanding of this template and document its potential/limitations as a reusable asset for future, specialized client projects, leveraging Cursor to accelerate both learning and development.

**2. Core Objectives (Ongoing)**

*   **Deep Understanding (via Cursor Ask):**
    *   Maintain an up-to-date understanding of the template's architecture, key components, data flow, styling, and configuration.
    *   Identify and document reusable UI patterns and customization hooks within the template.
    *   Quickly onboard team members or refresh knowledge using targeted Ask queries.
*   **Rapid Prototyping & Adaptation (via Cursor Agent):**
    *   Efficiently prototype UI modifications based on hypothetical client needs or brainstorming sessions.
    *   Use Agent to generate boilerplate for new schema types and their corresponding UI components within the template's structure.
    *   Experiment with refactoring sections of the template for improved clarity, performance, or adaptability using Agent guidance.
    *   Test the template's flexibility by instructing Agent to implement small, novel UI features relevant to potential AI niches.
*   **Niche Applicability Assessment:**
    *   Continuously evaluate how easily the template's structure and components can be adapted for specific AI-related workflows (e.g., managing prompts, reviewing AI outputs, visualizing relationships in AI-generated data).
    *   Document successful (and unsuccessful) Agent-driven adaptations relevant to these niches.

**3. Scope**

*   **In Scope:**
    *   **Understanding (Ask):** Any part of the template's codebase (React components, schemas, config, styling).
    *   **Modification (Agent):** Prototyping UI changes, adding/modifying schema-component mappings, refactoring existing components, generating boilerplate, experimenting with styling changes, implementing small new features relevant to brainstorming.
    *   **Documentation:** Capturing key findings, successful patterns, customization guides, and results of Agent-driven experiments.
*   **Out of Scope (Unless explicitly decided otherwise):**
    *   Full production-ready feature development (Agent is for prototyping/assistance).
    *   Large-scale architectural changes without significant manual oversight.
    *   Performance optimization beyond basic refactoring suggestions.
    *   Deploying prototyped versions.

**4. Key Exploration & Modification Areas (Examples for Cursor Interaction)**

*(Use these as starting points, adapt based on findings)*

*   **Understanding (Cursor Ask - `Cmd+K`, Chat):**
    *   `Ask:` "Explain the props and state management in `[ComponentName].js`."
    *   `Ask:` "Trace how the value for the `[field_name]` field in the `[schema_name]` schema is passed to its input component and how updates are sent back."
    *   `Ask:` "Summarize the purpose of the Sanity `parts` overrides defined in `sanity.config.js` related to the UI."
    *   `Ask:` "How is styling applied to components in the `[directory_path]` directory? What's the primary method (CSS Modules, Styled Components, etc.)?"
    *   `Ask:` "Identify the main layout components used by this template."
    *   `Ask:` "What are the key configuration options available for `[SpecificPluginOrComponent]`?"
*   **Modification & Prototyping (Cursor Agent - `Cmd+Enter`, Chat):**
    *   `Agent:` "Refactor `[ComponentName].js` to use React Hooks instead of class components (if applicable)."
    *   `Agent:` "Generate a new schema file named `aiPrompt.js` with fields for 'promptText' (text), 'modelUsed' (string), 'parameters' (object), and 'generatedOutput' (portable text). Also, create a basic React component `AiPromptInput.js` to render this and integrate it into the schema definition."
    *   `Agent:` "Modify the styling in `[ComponentStyles.css/js]` to change the primary color to `#FF5733`."
    *   `Agent:` "Add a simple 'Copy to Clipboard' button next to the `[field_name]` input in `[ComponentName].js`."
    *   `Agent:` "Implement basic conditional rendering in `[ComponentName].js`: if the `status` field is 'approved', show a green checkmark icon."
    *   `Agent:` "Prototype a simple list view component that displays all documents of type `[schema_name]` within this template's UI structure."

**5. Brainstorming Prompts for Niche AI Applications (Using Codebase Context)**

*(Leverage Cursor's codebase awareness during brainstorming)*

*   `Ask/Agent:` "Given the structure of `[ComponentName].js` which handles `[field_type]`, how could we adapt it to include a button that sends the field's content to an external AI API and displays the result?" (Use Agent to prototype the UI change).
*   `Ask:` "Based on the schema definitions, what's the best way to model a relationship between user prompts (`aiPrompt` schema) and their generated results (`aiResult` schema) within this template's capabilities?"
*   `Agent:` "Generate a UI component that allows side-by-side comparison of two Portable Text fields, potentially for reviewing original vs. AI-edited content. Integrate it for a hypothetical `contentReview` schema."
*   `Ask:` "How could we leverage the existing array input component structure to manage a list of parameters for an AI model configuration?"
*   `Agent:` "Prototype a simple dashboard view within the Studio using this template's components that shows statistics about AI content generation (e.g., number of prompts, average generation time - using dummy data)."

**6. Documentation Strategy (Ongoing)**

*   Maintain this PRD as the central guide.
*   Use comments within the code (potentially aided by Cursor) to explain complex sections identified via Ask.
*   Create separate Markdown files (or use a wiki/Notion) to document:
    *   Key architectural patterns discovered.
    *   Step-by-step guides for common customizations (informed by successful Agent modifications).
    *   Summaries of successful/failed Agent-driven experiments related to AI niches.
    *   A "Cookbook" of useful Cursor Ask/Agent prompts specific to this codebase.
*   Use Cursor's ability to generate documentation snippets where appropriate.

**7. Success Looks Like (Ongoing)**

*   Team members can quickly understand and navigate the codebase using Cursor Ask.
*   We can rapidly prototype UI changes and adaptations using Cursor Agent.
*   We have documented, reusable patterns for customizing the template.
*   We have a growing list of documented experiments showing how the template can (or cannot) be adapted for specific AI-driven client needs.
*   This codebase becomes a tangible asset that accelerates brainstorming and quoting for relevant niche projects.

**8. Open Questions & Future Exploration Areas**

*   [Track specific technical questions as they arise]
*   [List potential AI niches to explore further, e.g., AI Writing Assistant UI, Data Annotation Tooling, Prompt Engineering Interface]
*   How well does the template handle real-time collaboration features if needed?
*   What are the performance characteristics under heavy customization?

---

This PRD provides a framework for continuous learning and adaptation. Treat it as a living document, updating it as you discover more about the codebase and refine your ideas for niche applications, always keeping Cursor's Ask and Agent capabilities central to the workflow.