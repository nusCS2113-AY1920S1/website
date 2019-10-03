{% macro show_main_text() %}
<div id="main">

<div id="title">

</div>
<div id="body">

<p class="lead" style="color: purple"><md>:far-calendar-check: <include src="project-timeline.md#mid-v12-overview" inline /></md><p/>

**<big>Project Management:</big>**

<box>

:bulb: **You are free to adjust _process rigor_ and _project plan_ at any future time in the project**, starting from v1.2.  
If you are not sure if a certain adjustment is allowed, you can check with the lecturer first.
</box>


* **Adjust process rigor to suit your team's pace:**  
  * **Switch to a lighter workflow:** While forking workflow is the safest, it can be heavy. You can switch to a simpler workflow if the forking workflow is slowing you down.  
  Refer the textbook to find more about alternative workflows: branching workflow, centralized workflow.  
  However, we still recommend that you use PR reviews, at least for PRs affecting others' features.  
  * **Reduce automated checks**: You can also reduce the rigor of checkstyle checks to expedite PR processing.  
  * **You can also increase the rigor/safety of your workflow** in the following ways:
    * Use GitHub's [_Protected Branches_](https://help.github.com/articles/about-protected-branches/) feature to protect your `master` branch against rogue PRs.  

* **Adjust project plan if necessary**. By now you will have a some idea about the code base and the product that you envisoned. You can revisit the feature release plan and adjust it if necessary.

* %%(If you haven't already done)%% Set up the issue tracker:

<div class="indented-level2">

{{ embed_topic("appendixE-gitHub.md#issue-tracker-setup", "Admin " + icon_embedding + " Appendix E(extract): **Setting up the issue tracker**", "midv12-issueTrackerSetup", "1") }}
</div>


* %%(If you haven't already done)%% Start proper schedule tracking and milestone management:

<div class="indented-level2">

{{ embed_topic("appendixE-gitHub.md#project-schedule-tracking", "Admin " + icon_embedding + " Appendix E(extract): **Project schedule tracking**", "midv12-projectScheduleTracking", "1") }}
</div>

<div id="product">

**<big>Product:</big>**

* **From v1.2 onwards each member is expected to contribute <tooltip content="the amount of code does not matter; even small contributions are acceptable">some</tooltip> code to each <tooltip content="v1.2, v1.3, v1.4"> milestone</tooltip>, preferably each week; only merged code is considered as contributions** %%<popover content="The ability to deliver code incrementally is an important learning outcome of this module because incremental delivery improves the _visibility_ of your work.">(Reason)</popover>%%. <br>
 If an enhancement is too big to complete in one milestone, try to deliver it in smaller incremental steps e.g. deliver a basic version of the enhancement first.


</div>

<!--



* **Switch to AB-3 or AB-2 if AB-4 is not working out for you**.

<div class="indented-level2">

{{ embed_topic("project-deliverables.md#notes-for-ab23", "Admin " + icon_embedding + " Project Deliverables → Notes for Those Using AB-2 or AB-3 for the Project", "midv12-notesForAb23", "3") }}
</div>


<div class="indented-level2">

{{ embed_topic("appendixE-gitHub.md#workflow-after-v11", "Admin " + icon_embedding + " Appendix E(extract): **Workflow (after v1.1)**", "midv12-workflowAfterV11", "3") }}
</div>




-->

</div>
</div>
{% endmacro %}

{% from "common/macros.njk" import embed_topic with context %}
{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("project-w08-mid-v12", show_main_text) }}