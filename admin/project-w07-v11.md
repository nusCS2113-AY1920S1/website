{% macro show_main_text() %}
<div id="main">

<div id="title">

</div>
<div id="body"> 



<p class="lead" style="color: purple"><md>:far-calendar-check: <include src="project-timeline.md#v11-overview" inline /></md></p>



{{ icon_important_big_red }} **Milestone progress is graded**. Be reminded that reaching individual and team milestones are considered for <trigger trigger="click" for="modal:v11-projectMgtGrading">grading the _project management_ component</trigger> of your project grade.

{{ icon_important_big_red }} **Most aspects project progress are tracked using automated scripts.** ==Please follow our instructions closely or else the script will not be able to detect your progress==. We prefer not to spend admin resources processing requests for partial credit for work that did not follow the instructions precisely, unless the progress was not detected due to a bug in the script.

{{ icon_important_big_red }} **Milestone requirements are cumulative**. The recommended progress for the mid-milestone is an implicit requirement for the actual milestone unless a milestone requirement overrides a mid-milestone requirement %%e.g., mid-milestone requires a document to be in a temp format while the actual milestone requires it to be in the proper format%%. Similarly, a requirement for milestone `n` is also an implicit requirement for milestone `n+1` unless `n+1` overrides the `n` requirement. This means ==if you miss some requirement at milestone `n`, you should try to achieve it before milestone `n+1`== or else it could be noted again as a 'missed requirement' at milestone `n+1`.

{{ icon_important_big_red }} **Deadline**. As all other things so far, the deadline for achieving the milestones is the midnight before your tutorial. %%(E.g., Wednesday teams should complete the milestone by Tuesday 2359 hrs)%%.

**v1.1 Summary**

Milestone | Minimum acceptable performance to consider as 'reached'
--------- | -------------------------------------------------------
{{ icon_team }} Team org/repo set up | as stated in <trigger trigger="click" for="modal:v10setup-v10">Week 5</trigger>
{{ icon_individual }} Some code enhancements done | created PRs to do local/global changes
{{ icon_individual }} Photo uploaded | a photo complying to <trigger trigger="click" for="modal:v11-photo">our guidelines</trigger> is in the master branch of your team repo
{{ icon_team }} Project docs updated | updated docs are merged to the master branch
{{ icon_team }} Milestone wrapped up | a commit in the master branch tagged as `v1.1`; milestone closed on GitHub


<modal large title="Admin {{ icon_embedding }} Project: v1.0 - Setup" id="modal:modal:v10setup-v10">
  <include src="project-w05-v10.md#project_setup"/>
</modal>

<modal large title="Admin {{ icon_embedding }} Project Assessment → Project Management" id="modal:v11-projectMgtGrading">
  <include src="project-assessment.md#project-management-grading"/>
</modal>

<modal large title="Admin {{ icon_embedding }} Choosing a profile photo" id="modal:v11-photo">
  <include src="project-deliverables.md#profile-photo"/>
</modal>

<br>

<div id="documentation">

### v1.1 Project Management

* {{ icon_team }} Fix any errors in org/repo set up %%&nbsp;(e.g. wrong repo name)%%.
* **Wrap up the milestone using a git tag `v1.1`** as explained below:
  * When the milestone deadline is near (e.g., 0.5 days before the deadline), if you think some of the ongoing work intended for the current milestone may not finish in time, reassign them to a future milestone.
  * After all changes that _can_ be merged before the milestone deadline has been merged, use `git tag` feature to tag the current version with the milestone and push the tag to the team repo.
  * Close the milestone on GitHub explicitly.


### v1.1 Documentation

* Update User Guide, Developer Guide, README, and About Us pages as described earlier in <trigger trigger="click" for="modal:v11docs-midv11">mid-v1.1 progress guide</trigger>.

  **Submission**:
    * Submit two pdf files on LumiNUS, one for the user guide and the other for the developer guide.
    * The **user guide** should have the concrete command syntax and explanation for features that you would implement (in v1.4) and the features that are planned for v2.0
    * The **developer guide** should have the <trigger trigger="click" for="modal:v10docs-v10">user profile, value proposition and Appendix A containing user stories, use cases and NFR.</trigger>.

<modal large title="Admin {{ icon_embedding }} Project: mid-v1.1" id="modal:v11docs-midv11">
  <include src="project-w06-mid-v11.md#documentation"/>
</modal>

<modal large title="Admin {{ icon_embedding }} Project: Phase 2" id="modal:v10docs-v10">
  <include src="project-w05-v10.md#project_phase2"/>
</modal>

</div>
<div id="product">

### v1.1 Product

**Suggested approach to development:**

* First, each member can attempt to do a <tooltip content="a change impacting only one component">local-impact</tooltip> change to the code base. <br>
  **Objective**: To familiarize yourself with at least one <tooltip content="components as stated in the [Developer Guide: Architecture]">components</tooltip> of the product. <br>
  **Description**: Divide the components among yourselves. Each member can do some small enhancements to their component(s) to learn the code of that component.

* Further, each member should try to add some enhancements that are in line with the vision for v2.0. After adding some _local-impact_ changes recommended above, attempt to do some ==<tooltip content="should go beyond the component you are in charge of">_global-impact_</tooltip> enhancements==, touching as many other components as possible.

  **Submission**:
    * Create PRs from your own fork to your team repo. Get it merged by following your team's workflow.
    
</div>

<!--

 Refer to the AddressBook-Level4 Developer Guide has [some guidance on how to implement a new feature end-to-end](https://nus{{ module | lower }}-{{ semester | lower }}.github.io/addressbook-level4/DeveloperGuide.html#GetStartedProgramming-RemarkCommand).
 
  <include src="project-w06-mid-v11.md#body"/>project_setup
-->

</div>
</div>
{% endmacro %}

{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("project-w07-v11", show_main_text) }}
