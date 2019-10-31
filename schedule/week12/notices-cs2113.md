{% from "schedule/index.md" import show_week_pagetop with context%}
{{ show_week_pagetop(12, "notices") }}

## Demo during tutorial

- The remaining members (who did not demo the previous week) do a timed demo in the tutorial this week
- Ensure that you have at least 20 **meaningful** data items (%%Reason: your demo doesn't look good if the app is blank!%%
  - E.g., `aaa`, `test 1`, etc., are not considered meaningful
- Be aware of the requirements of [v1.4 submission](https://nuscs2113-ay1920s1.github.io/website/admin/project-w13-v14.html)

## Mock MCQ

- We will have a mock MCQ test in the last 30 min of the lecture, just for you to gain some practise.
- This is not graded.

## Prepare testing instructions
 
* You need to create a new section in the **appendix** of your DG, named _Instructions for Manual Testing_. It should include testing instructions to **cover the features of each team member**.<br>
  
* **What to include** in the _Instructions for Manual Testing_?  
  This appendix is meant to give some guidance to the tester to chart a path through the features, and provide some important test inputs the tester can copy-paste into the app.  
  There is no need to give a long list of test cases including all possible variations. It is upto the tester to come up with those variations.  
  However, if the instructions are inaccurate or deliberately misses/mis-states information to make testing harder %%&nbsp;i.e. annoys the tester%%, the tester can report it as a bug %%&nbsp;(because flaws in developer docs are considered as bugs)%%.
  
* If the _Instructions for Manual Testing_ is missing in your DG during the final testing session, the tester flags it as a high severity documentation bug.