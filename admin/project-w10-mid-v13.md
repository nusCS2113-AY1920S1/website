{% macro show_main_text() %}
<div id="main">

<div id="title">

</div>
<div id="body">

<p class="lead" style="color: purple"><md>:far-calendar-check: <include src="project-timeline.md#mid-v13-overview" inline /></md></p>

**<big>Submission</big>**

* Submit the **updated developer guide (pdf)** this week on LumiNUS.
* Ensure that you follow the proper naming convention.
  * The file name should be `[Team id]-Product name-DG.pdf` e.g., `[AY1920S1-CS2113T-F10-3]-ProDuke-DG.pdf`
  * %%While we won't penalize you now, you will be penalized for not adhering to the naming convention in your final submission%%

**<big>Product:</big>**

* {{ icon_important_big_red }} **Do a <tooltip content="resulting in a jar file on GitHub that can be downloaded by potential users">proper product release</tooltip>** [as described in the reference project DevOps page](https://github.com/nusCS2113-AY1920S1/addressbook-level3/blob/master/docs/DevOps.adoc#5-making-a-release). 
 You can name it something like `v1.2.1`.  
 ==Ensure that the jar file works as expected== by doing some manual testing.  
 %%Reason: You are _required_ to do a proper product release for v1.3. Doing a trial at this point will help you iron out any problems in advance.  
 It may take additional effort to get the jar working especially if you use third party libraries or additional assets such as images.%%


**<big>Documentation:</big>**

* **User Guide**: Update where the document does not match the current product.
* **Developer Guide**:   
  * ==Each member should describe the implementation of at least one enhancement (s)he has added== (or planning to add). <br>
      Expected length: 1+ page of technical content per person
    * The description can contain things such as,
      * How the feature is implemented.
      * Why it is implemented that way.
      * Alternatives considered.
    * The stated objective is to explain the implementation to a future developer, but a hidden objective is to show evidence that you can document deeply-technical content using prose, examples, diagrams, code snippets, etc. appropriately. To that end, you may also describe features that you plan to implement in the future, even beyond v1.4 (hypothetically).
    * For an example, see [the description of the undo/redo feature implementation in the reference project's developer guide](https://github.com/nusCS2113-AY1920S1/addressbook-level3/blob/master/docs/DeveloperGuide.adoc#proposed-undoredo-feature).
  * Move the user stories, use cases and NFR under Appendix: Requirements



**<big>Project Management:</big>**

* Continue to do deliberate project management using GitHub issue tracker, milestones, labels, etc. as you did in v1.2.
* :bulb: We recommend that **each PR also updates the relevant parts of documents and tests**. That way, your documentation/testing work will not pile up towards the end.
* :bulb: There is [a way to get GitHub to auto-close the relevant issue when a PR is merged](https://help.github.com/articles/closing-issues-using-keywords/) ([example](https://github.com/se-edu/addressbook-level4/pull/888)).

**Ensure your code is <tooltip content="i.e., RepoSense can detect your code as yours">RepoSense-compatible</tooltip>**, as explained below:

<panel type="seamless" header="#### Ensuring your code is RepoSense-Compatible" expanded >
  <include src="reposenseCompatibility.md#main" />
</panel>

</div>
</div>

{% endmacro %}

{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("project-w10-mid-v13", show_main_text) }}