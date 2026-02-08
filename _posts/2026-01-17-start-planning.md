---
title: "How do I plan for a task?"
---



Here are the steps when I am doing requirement analysis and system design



- Read through the requirements in any format

- Understand the business goal 

- Draw out the process flow by answering following questions step by step

  - Who
  - What
  - When
  - Where
  - How

- Identify the key concepts in the content

  - Actors
  - Systems
  - Business Entities

- Refer to existing domain model to rename the entities in the process flow

- Identify the new concepts and name them to avoid the conflict with existing domain entities

- Draw out collaboration diagram from the process flow by referring to the requirement to avoid missing information

- Use process flow and collaboration diagram to match the minimum process scope.

  - This may lead to a master data model to provide global context other than finding the bigger scope as necessary
  - To facilitate this goal, we may need to host a domain-model under each process.

- Merge the process to existing process. The new process description may have the steps in different depth, some of them may be the steps in a sub-process. We should figure them out intelligently.

- Find the top node of the process in the merged, update process diagram, collaboration diagram and domain-model diagram accordingly by traversing the tree to further depth.

- The new message in the diagram is the new sub-process. If there no further detail of it being describe, we are not going to break it down further.

- Identify the tasks. Once we have completed the above process, we are able to find out all the processes which needs to be modified and created. These are the tasks we need to do. They have the dependencies from bottom to top.

- Estimate the efforts for the tasks.

- Put the effort estimates and the tasks dependency together to make up a project plan.


Below is the **English translation** of the methodology explanation (originally summarized in Chinese). I’ve preserved the structure and intent, and clarified a few terms for readability.

***

## Methodology Overview (English Translation)

This methodology is used for **system analysis** and **business process modeling**. Its core steps are:

### 1) Goal Identification & Process Mapping

*   Clarify the overall **system/business objectives**, typically via interviews with business experts (e.g., Business Analysts—BA, Subject Matter Experts—SME).
*   Map the **current business process**, identify key steps and participating departments, and produce a **high‑level process diagram** (e.g., flowchart or collaboration diagram).

### 2) Context and Boundary Definition

*   Emphasize the importance of **context** (termed “时境” in Chinese), explicitly defining **system boundaries** and the interactions among subsystems.
*   Use **process diagrams** and **interaction/collaboration diagrams** to show collaboration and information flows inside and outside the system.

### 3) Requirements Elicitation and Normalization

*   Gather **raw requirements** (often verbal or unstructured) and convert them into **standardized artifacts** (e.g., **User Stories**, **Functional Requirement Documents**).
*   Apply the **Golden Circle** (Why → How → What) to uncover the real intent behind each request and avoid focusing only on feature details.

### 4) Process Detailing and Decomposition

*   Iteratively **decompose complex processes** into manageable sub‑processes and tasks to reduce overall complexity.
*   Use diagrams (e.g., flowcharts, use case/sequence/collaboration diagrams) to detail logic, **conditional branches** (binary and multi‑branch), and **loops**.

### 5) Documentation and Visual Expression

*   Combine **standardized documentation** and **diagrams** to express business logic in ways that are easy for development teams to understand and implement.
*   Stress **text‑and‑visual pairing**: diagrams for structure and flow; text for rules, edge cases, and acceptance criteria.

### 6) Continuous Iteration and Optimization

*   Compare **current** vs. **future (to‑be)** processes, continually refining workflows and system design.
*   Leverage **AI tools** to assist with modeling, documentation generation, and requirement analysis to improve efficiency and accuracy.

***

### Notes on Practices Mentioned

*   **Artifacts & Notation:** Flowcharts for procedural flow; collaboration/sequence diagrams for inter‑system or human‑system interaction; User Stories with acceptance criteria for testable requirements.
*   **Stakeholder Roles:** SMEs provide domain knowledge; BAs translate raw needs into structured, development‑ready specifications.
*   **Design Principle:** Design turns a complex problem into several simpler problems that different roles can solve collaboratively.
*   **AI Assistance:** Use AI to transform diagrams, generate documentation drafts, and maintain consistency between visual models and textual specs.

***

### 方法论中文总结

本方法论主要用于系统分析和业务流程建模，核心步骤如下：

1.  **目标识别与流程梳理**
    *   明确系统或业务的总体目标，通常通过与业务专家（如BA、SME）访谈获得。
    *   梳理现有业务流程，识别关键步骤和参与部门，形成高层流程图（如flowchart、协作图）。

2.  **上下文与边界定义**
    *   强调“上下文”（实境）的重要性，明确系统边界和各子系统的交互关系。
    *   通过流程图和交互图，展现系统内外部的协作与信息流。

3.  **需求收集与规范化**
    *   收集原始需求（raw requirement），将口头或非结构化需求转化为标准化文档（如User Story、Functional Requirement Document）。
    *   采用“黄金圈法则”（Why-How-What）深入挖掘需求本质，避免只关注细节功能。

4.  **流程细化与分解**
    *   将复杂流程逐层分解为可管理的小流程和任务，降低整体复杂度。
    *   通过流程图、用例图等工具，细化每个环节的逻辑、条件分支和循环。

5.  **文档与可视化表达**
    *   用规范化文档和流程图表达业务逻辑，便于开发团队理解和实现。
    *   强调图文结合，流程图用于整体把控，文字描述补充细节。

6.  **持续迭代与优化**
    *   当前流程与未来流程对比，持续优化业务流程和系统设计。
    *   利用AI工具辅助流程建模、文档生成和需求分析，提高效率和准确性。

***

### English Optimized Prompt for System Analysis (Applying the Methodology)

**Your Optimized Prompt:**

> **Role:** You are a senior system analyst specializing in business process modeling and requirements engineering.
>
> **Context:** You are tasked with analyzing and optimizing the workflow of a given enterprise system. The goal is to clarify objectives, map current processes, and identify opportunities for improvement.
>
> **Methodology:**
>
> 1.  **Goal Identification:** Interview stakeholders to define the overall system/business objectives.
> 2.  **Context & Boundary Definition:** Clearly outline system boundaries and the interactions between subsystems using flowcharts and collaboration diagrams.
> 3.  **Requirements Gathering:** Collect raw requirements and convert them into standardized documentation (e.g., User Stories, Functional Requirement Documents). Apply the "Golden Circle" approach (Why-How-What) to uncover the true purpose behind each requirement.
> 4.  **Process Decomposition:** Break down complex workflows into manageable sub-processes and tasks, using diagrams to illustrate logic, conditions, and loops.
> 5.  **Documentation & Visualization:** Combine visual diagrams and textual descriptions to communicate business logic and requirements to the development team.
> 6.  **Continuous Iteration:** Compare current and future processes, iteratively refine workflows, and leverage AI tools for modeling and documentation.
>
> **Output Requirements:**
>
> *   Provide a high-level process map (flowchart) of the current workflow.
> *   Summarize key requirements in standardized format (e.g., User Stories).
> *   Identify areas for process improvement and propose actionable recommendations.
> *   Document all findings in a clear, structured report suitable for both business and technical audiences.
>
> **Constraints:**
>
> *   Ensure all diagrams and documentation are easy to understand for non-technical stakeholders.
> *   Maintain traceability between requirements, process steps, and system objectives.

**Key Improvements:**
• Structured methodology for system analysis
• Explicit role assignment and output requirements
• Integration of visual and textual documentation
• Emphasis on stakeholder interviews and iterative refinement

**Techniques Applied:**  
Role assignment, context layering, process decomposition, Golden Circle questioning, diagram-based modeling, documentation standards

**Pro Tip:**  
Use AI tools to automate diagram generation and requirements documentation, ensuring consistency and saving time during analysis.


  

