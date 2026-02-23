---
title: "First iteration is done"
---

I have implemented a full set of skills from requirement analysis to planning. The project plan and task breakdowns can make the project kick off.

I used a real project BRD as start point, only one round skill run and one feedback to change the implementation strategy. The project plan and design model are generated in a pretty good shape

Issues I can see so far 

- Task estimate is not accurate, each task has comprehensive sub tasks created. However, the human developer is not able to complete the tasks in the estimated timeframe.
- Existing infrastructure and services have not integrated yet.
- The orgModel hierarchy has not been created, currently the structure is flat.
- Progress tracking. If we use huamn developer work on this, it is not feasible to update the task progress based on the code committed. Mannual progress update is time consuming.
- Test cases are identified but not detailed enough for QA. Test case is the way to elaborate user requirement in detail as its role in EDPS.


Further improvements I can consider towards my ultimate goal - Evolutionary Development

- Build skills to allow engaging existing infrasture and services
- Improve the modeling skills to create the model document hierarchy by following EDPS methodology
- Build skills to integrate with GitHub. 
  - Tasks can be posted in GitHub project 
  - Tasks can synchronize with the progress update.  
  - Tasks can be accomplished by GitHub copliot
- Build coding agent, system configuration agent, testing agent.
- Build skills to generate comprehensive test cases
- Build mechanism to allow iteration output being fed back to next iteration. We need always to make adjustments to the AI output to assure the project evolution towards the direction we expect.