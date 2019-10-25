{% from "schedule/index.md" import show_week_pagetop with context%}
{{ show_week_pagetop(11, "notices") }}

## Project

- This week, you need to create a a release for your product, with a JAR.
- Ensure that the product is user testable.
- Update the documents to reflect the state the product. 
  - Mark irrelevant sections as `coming in v2.0`.

#### User testing session
<include src="../../admin/project-testing.mbdf#testingPreparations" />
 
## Demo during tutorial

- Two members do a timed demo in the tutorial this week. (Come prepared for demo!)

## (Mock) Submissions this week

* Submit the following documents on LumiNUS.
  * Ensure that the file names are accurate. While there is no penalty now for non-compliance, you will lose marks for making similar mistakes in the final submission.
* ==The submission folder `Project submission v1.3` will be open from Oct 29, 2019 00:00 am to Oct 31, 2019 11:59 pm==

Team/Individual Item | Name format | Upload to
-------------------- | ----------- | ---------
{{ icon_team }} User Guide | `[TEAM_ID]-[product Name]-UG.pdf`<br>  %%e.g.`[AY1920S1-CS2113T-F10-3]-ProDuke-UG.pdf`%% | LumiNUS
{{ icon_team }} Developer Guide | `[TEAM_ID]-[product Name]-DG.pdf`<br> %%e.g. `[AY1920S1-CS2113T-F10-3]-ProDuke-DG.pd`f%% | LumiNUS
{{ icon_individual }} Project Portfolio Page | `[TEAM_ID]-[Your Name]PPP.pdf`<br> %%e.g.`[AY1920S1-CS2113T-F10-3][John Doe]PPP.pdf`%% | LumiNUS

## FAQ for Reposense



1. My contributions are not detected in the reposense report, why?
    1. Check:
        1. Have you set the `user.name` to your GitHub user name that you provided in the pre-module survey?
        1. Have you used different git user name while doing the work? Run `git log` command on the command line/terminal and look for the `Author` field.
    1. If the above are correct, you should provide the additional names appearing on `git log` to the lecturer.   
      
1. I have done everything given in 1, but I still can't see my contributions. How to resolve?
    1. Use `@@author` tags to identify your code contribution in the source files.
    1. Follow the instructions given in the reposense documentation for this
    1. Specifically, don't put `@@author` tags inside Javadoc comments, it should be placed before the Javadoc comments.
    
1. I did 1 & 2, however, I cannot still see my contributions. Help!!
    1. Usually, most cases will be taken care of by 1 and 2 above. 
    1. In case your contributions are still not detected, please post the issue on this forum, we will get the reposense team to take a look.

1. How frequently is the reposense report generated?
   1. Reposense is configured to run the report everyday.

1. My friend and I worked on a piece of code together, but only my friend committed. Now how?
    1. Use `@@author` tags to indicate chunks of the file that is your contribution. Arrive at a consensus with your friend/teammate before claiming part of the code as yours.

1. What is considered **good contribution**?
    1. Speaking from code-quality evaluation perspective, you need to have contiguous code chunks in your contribution (e.g., some full classes, some significantly long full methods).
    1. If the code is fragmented (e.g., you only added one additional field to a class, and the entire code has fragmented one-two lines that work with the additional field you creates) it becomes hard to grade the code quality.


