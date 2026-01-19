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

  

