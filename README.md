# Agent-Ready Jira Story Template 🤖🎯

Welcome to the **Agent-Ready Jira Story Template** repository! This project provides a structured, highly optimized markdown template designed specifically to bridge the gap between human requirements and AI developer execution.

Whether you are using coding assistants (like Gemini, Claude, or Copilot), autonomous agents (like Devin or Antigravity), or custom internal triage bots, this template ensures your agents have the context, constraints, and instructions they need to work correctly on the **first attempt** without hallucinations.

---

## 📖 Why Do We Need "Agent-Ready" Stories?

Traditional Jira stories are often written for humans who possess implicit context, institutional knowledge, and the ability to ask quick clarifying questions. 

When an AI agent takes on a ticket with ambiguous instructions, it is highly prone to:
*   **Scope Creep & Code Churn:** Refactoring unrelated components.
*   **Hallucinations:** Inventing utility functions or backend APIs that do not exist.
*   **Constraint Violations:** Using unauthorized packages, changing database schemas, or ignoring styling guidelines.
*   **Broken Builds:** Completing the task but failing to run tests or comply with the project's verification suite.

By structuring Jira stories with specific constraints, system boundaries, and Gherkin-style acceptance criteria, you turn your tickets into **machine-executable specifications**.

---

## 🛠️ The Core Components

An Agent-Ready story divides requirements into structured sections designed to maximize LLM parseability:

| Section | Target Purpose | Why Agents Need It |
| :--- | :--- | :--- |
| **1. Context & Objectives** | User story & problem statement. | Helps the agent understand the high-level intent to make smart micro-decisions. |
| **2. Technical Scope** | Specific target files and components. | Restricts the agent's attention and edit boundaries to prevent unrelated codebase churn. |
| **3. Acceptance Criteria** | Gherkin format (`Given/When/Then`). | High-precision logical paths that agents can directly compile into unit or integration tests. |
| **4. Technical Constraints** | Do's and Don'ts checklist. | Hard boundaries (e.g. "Do not install dependencies", "Use Tailwind only"). |
| **5. Verification Steps** | Command lines for testing/linting. | Defines the exact validation commands the agent must run to verify its work. |
| **6. References** | API payloads, Figma designs, docs. | Feeds the agent raw schemas, avoiding the need for it to guess structures. |

---

## 🚀 How to Use

1. **Copy the Template:** Copy the raw content from [AGENT_READY_JIRA_STORY_TEMPLATE.md](./AGENT_READY_JIRA_STORY_TEMPLATE.md).
2. **Configure Jira:**
   * Go to your Jira Project Settings.
   * Navigate to **Issue Layout** or **Issue Templates** (if using apps like *Jira Templates*).
   * Paste this markdown structure as the default description.
3. **Write with AI in Mind:** When creating a ticket, fill out each section. If a section is not applicable, state `N/A` rather than leaving it empty.

---

## 📝 Examples

Check out the following mock tickets in the `examples/` directory to see the template in action:
*   [Example 1: Bug Fix (Login Form Validation Bug)](./examples/example_bug_fix.md)
*   [Example 2: Feature Request (Theme Selector Toggle)](./examples/example_feature_request.md)

---

## 🤝 Contributing

Contributions to improve the template structure, add more examples, or write guides for specific AI tools are welcome! Feel free to open a Pull Request.
