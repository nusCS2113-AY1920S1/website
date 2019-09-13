{% macro show_main_text() %}
<div id="main">

<div id="title">

</div>
<div id="body">

<p class="lead" style="color: purple"><md>:far-calendar-check: <include src="project-timeline.md#mid-v11-overview" inline /></md><p/>

# Phase 2 Project tasks

<div id="documentation">

**<big>Documentation:</big>** 

<tip-box>

**Recommended:** Divide among yourselves who will update which parts of the document(s).

</tip-box>

* **User Guide**:  
  Start drafting a user guide in a convenient medium (e.g., a GoogleDoc) to describe what the product would be like when it is at v2.0. %%Which means, you can include commands that you may not implement in the project.%%
  * We recommend that you follow the [reference project's User Guide](https://github.com/nusCS2113-AY1920S1/addressbook-level3/blob/master/docs/UserGuide.adoc) in terms of structure and format.
  * As this is a beginning draft, don't waste time in formatting, copy editing etc. It is fine as long as the tutor can get a rough idea of the features from this draft. You can also do just the 'Features' section and omit the other parts.
  * Do try to come up with concrete command syntax for feature that you would implement (at least for those that you will implement by v1.4).
  * Consider including some UI mock-ups too %%(they can be hand-drawn or created using a tool such as PowerPoint or [Balsamiq](https://balsamiq.com/))%%.

* **Developer Guide**:  
  Update the developer guide (target user profile, user stories, use cases, and non-functional requirements) based on the feedback from your tutors.

**<big>Admin pages:</big>** 

<div class="indented">

  Create/update the following pages in your project repo:
</div> 
 
* Create the **_About Us_ page**:<br>
  Use [this page from the reference project](https://github.com/nusCS2113-AY1920S1/addressbook-level3/blob/master/docs/AboutUs.adoc) as a reference for the format.
  This page is used for module admin purposes. ==Please follow the format closely== or else our scripts will not be able to give credit for your work.
  * You may copy the page and replace info of SE-EDU developers with info of your team, including a ==suitable photo== as described <trigger trigger="click" for="modal:mid-v12-photo">here</trigger>.  
  * Including the name/photo of the supervisor/lecturer is optional. 
  * The photo of a team member should be `doc/images/githbub_username_in_lower_case.png` %%e.g. `docs/images/johndoe.png`%%. ==If you photo is in jpg format, name the file as `.png` anyway==.
  * Indicate the different roles played and responsibilities held by each team member. You can reassign these <trigger trigger="click" for="modal:midv11-rolesAndResponsibilities">roles and responsibilities %%(as explained in Admin {{ icon_embedding }} Project Scope)%%</trigger> later in the project, if necessary.

<modal large title="Admin {{ icon_embedding }} Choosing a profile photo" id="modal:mid-v12-photo">
  <include src="project-deliverables.md#profile-photo"/>
</modal>

<modal large title="Admin {{ icon_embedding }} Project Scope (extract): roles and responsibilities" id="modal:midv11-rolesAndResponsibilities">
  <include src="project-scope.md#roles"/>
</modal>


* **README** page: Update it to match your project.

  * Add a UI mockup of your intended final product.   
    Note that the ==image of the UI should be `docs/images/Ui.png`== so that it can be downloaded by our scripts. Limit the file to contain one screenshot/mockup only and ensure the new image is roughly the same `height x width` proportions as the original one. %%Reason: when we compile these images from all teams into one page ([example](https://nuscs2113-ay1819s2.github.io/website/admin/projectList.html)), yours should not look out of place.%%

  * The original `README` file (which doubles as the landing page of your project website) is written to read like a setup instructions page. You should ==restructure this page to look like the home page of a real product== (not a school project) targeting real users. %%&nbsp;e.g. remove the section on feedback and reference to duke issue tracker%% 

</div>
 
# :fas-code-branch: Pull Requests to your team organization

- Use PRs as the mechanism to implement the extensions this week.
  - Create PRs to **your team repo's master branch**.
- Have these PRs merged in your team repo.
- [**Only for this week**] create PRs with titles following the format: `[Team id]-<your github username>-<Extension id>`. Example: `[CS2113T-W12-1]-johndoe-A-Gradle`
  - After this week, you can create PRs with any meaningful title to continue working on your project
- Each team member should review another member's PR on GitHub.
- More details about the suggested workflow:
  {{ embed_topic("appendixE-gitHub.md#workflow", "Admin " + icon_embedding + " Appendix E(extract): **Workflow**", "midv11-workflow", "1") }}

# Duke tasks ({{ icon_team }} team)

- Starting this week, you will only work on your team repo. <br>
- As a team implement the following extensions.
  - Create PRs and have them merged in the team repo.
- Do note that the `A-*` extensions are useful in your project as well.
- As earlier, tag the extension and push your changes to your team repository's master branch once it has been merged.


### `A-*` Extensions

- Automate build process with Gradle in your project

<box>
<include src="dukeFragment.md" boilerplate var-header="**`A-Gradle`: Build automation with Gradle**" var-fragment="extensions.mbdf#A-Gradle" />
</box>

- Enforce code quality
  
<box>
<include src="dukeFragment.md" boilerplate var-header="**`A-CheckStyle`: Enforce code quality**" var-fragment="extensions.mbdf#A-CheckStyle" />
</box>

- Learn to release a JAR on GitHub
  - You need to create a JAR using Gradle and then drop the JAR in the release you make on GitHub
  - Title the release as `mid-v1.1`

<box>
<include src="dukeFragment.md" boilerplate var-header="**`A-Jar`: Make a release**" var-fragment="extensions.mbdf#A-Jar" />
</box>

- [Optional] Setup CI

<box>
<include src="dukeFragment.md" boilerplate var-header="**`A-Travis`: Continuous Integration**" var-tag="optional" var-fragment="extensions.mbdf#A-Travis" />
</box>

- [Optional] Learn to add a dependency and use a library in your project
  - Do note that you have to comply with the library usage guidelines (You can refer to the notices tab for this week)

<box>
<include src="dukeFragment.md" boilerplate var-header="**`A-Libraries`: External libraries**" var-tag="optional" var-fragment="extensions.mbdf#A-Libraries" />
</box>


## `B-*` Extensions



- Create a branch from the base code of your team project in your own forks to implement these extensions
- Create PRs to your team repo master branch to incorporate the contributions.
  - Each member must implement **at least one unique** `B-` extension
  - Ensure you write _some_ unit tests for these increments using JUnit
  
<box>
<include src="dukeFragment.md" boilerplate var-header="**`B-Reminders`: Reminders**" var-fragment="extensions.mbdf#B-Reminders" />
<include src="dukeFragment.md" boilerplate var-header="**`B-FindFreeTimes`: Free time slots**" var-fragment="extensions.mbdf#B-FindFreeTimes" />
<include src="dukeFragment.md" boilerplate var-header="**`B-ViewSchedules`: View schedules**" var-fragment="extensions.mbdf#B-ViewSchedules" />
<include src="dukeFragment.md" boilerplate var-header="**`B-DetectAnomalies`: Detect scheduling anomalies**" var-fragment="extensions.mbdf#B-DetectAnomalies" />
<include src="dukeFragment.md" boilerplate var-header="**`B-Snooze`: Snooze**" var-fragment="extensions.mbdf#B-Snooze" />
<include src="dukeFragment.md" boilerplate var-header="**`B-TentativeScheduling`: Tentative scheduling**" var-fragment="extensions.mbdf#B-TentativeScheduling" />
<include src="dukeFragment.md" boilerplate var-header="**`B-RecurringTasks`: Recurring task**" var-fragment="extensions.mbdf#B-RecurringTasks" />
<include src="dukeFragment.md" boilerplate var-header="**`B-DoAfterTasks`: Do-after tasks**" var-fragment="extensions.mbdf#B-DoAfterTasks" />
<include src="dukeFragment.md" boilerplate var-header="**`B-DoWithinPeriodTasks`: Time bound tasks**" var-fragment="extensions.mbdf#B-DoWithinPeriodTasks" />
<include src="dukeFragment.md" boilerplate var-header="**`B-FixedDurationTasks`: Fixed duration tasks**" var-fragment="extensions.mbdf#B-FixedDurationTasks" />
</box>



<!--




  * Update the link of the Travis _build status badge_ (<img src="https://travis-ci.org/se-edu/addressbook-level4.svg?branch=master" alt="Build Status">) so that it reflects the build status of your team repo.<br>
    For the other badges,
    * either set up the respective tool for your project (AB-4 Developer Guide has instructions on how to set up AppVeyor and Coveralls) and update the badges accordingly,
    * or remove the badge.

  * Acknowledge the original source of the code i.e. AddressBook-Level4 project created by SE-EDU initiative at `https://github.com/se-edu/`

* **User Guide**: Start moving the content from your User Guide (draft created in previous weeks) into the User Guide page in your repository. If a feature is not implemented, mark it as 'Coming in v2.0' ([example]({{module_org}}/addressbook-level4/blob/master/docs/UserGuide.adoc#encrypting-data-files-code-coming-in-v2-0-code)).

* **Developer Guide**: Similar to the User Guide, start moving the content from your Developer Guide (draft created in previous weeks) into the Developer Guide page in your team repository.

**<big>Product:</big>**

* Each member can attempt to do a <tooltip content="a change impacting only one component">local-impact</tooltip> change to the code base.

  **Objective**: To familiarize yourself with at least one <tooltip content="components as stated in the [Developer Guide: Architecture]">components</tooltip> of the product.

  **Description**: Divide the components among yourselves. Each member can do some small enhancements to their component(s) to learn the code of that component. Some suggested enhancements are given in the [AddressBook-Level4 developer guide](https://nus{{ module | lower }}-{{ semester }}.github.io/addressbook-level4/DeveloperGuide.html#GetStartedProgramming-EachComponent).

  **Submission**: Create PRs from your own fork to your team repo. Get it merged by following your team's workflow.


</div>

-->

</div>
</div>
{% endmacro %}

{% from "common/macros.njk" import embed_topic with context %}
{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("project-w06-mid-v11", show_main_text) }}
