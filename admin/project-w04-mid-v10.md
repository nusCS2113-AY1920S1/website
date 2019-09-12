{% macro show_main_text() %}
<div id="main">

<div id="title">

</div>
<div id="body">

<p class="lead" style="color: purple"><md>:far-calendar-check: <include src="project-timeline.md#mid-v10-overview" inline /></md></p>

### Implement the following increments while committing code incrementally

Implement the following <tooltip content="in this context, an _increment_ is a Duke _level_ or a Duke _extension_">increments</tooltip> as per the instructions below.
  * Implement `Level-6` in a branch named `branch-Level-6`.
  * Without merging that branch, go back to the master branch and implement `Level-9` in a separate branch named `branch-Level-9`.
  * Now, go back to the master branch and merge the two branches one after the other.
 
  * Tag the commit (in the master branch, after merging) that achieves the respective deliverable.
  * As before, push to your fork.     
     
<br>

- Provide the capability to delete items from Duke's task list
  - Remember `Level-6` includes `A-Collections`

<box>
<include src="dukeFragment.md" boilerplate var-header="**`Level-6`: Delete**" var-fragment="text.md#level6" />
<include src="dukeFragment.md" boilerplate var-header="**`A-Collections`: Use Java Collection classes**" var-fragment="extensions.mbdf#A-Collections" />
</box>

- Do some automated testing of the Duke UI

<box>
<include src="dukeFragment.md" boilerplate var-header="**`A-TextUiTesting`: Text UI Testing**" var-fragment="extensions.mbdf#A-TextUiTesting" />
</box>

- Provide the capability to search for tasks that were recorded

<box>
<include src="dukeFragment.md" boilerplate var-header="**`Level-9`: Find**" var-fragment="text.md#level9" />    
</box>

- Make your code more object-oriented

<box>
<include src="dukeFragment.md" boilerplate var-header="**`A-MoreOOP`: More OOP**" var-fragment="extensions.mbdf#A-MoreOOP" />
</box>

- [Optional] Some members in the team: develop a GUI for Duke.
  - You will learn how to use JavaFX in `A-JavaFx`
  - If you plan to implement a GUI in your project Phase 2, it is recommended that at least one person in the team attempt this exercise successfully. 
  
<box>
<include src="dukeFragment.md" boilerplate var-header="**`Level-10`: GUI**" var-tag="optional" var-fragment="text.md#level10" />
<include src="dukeFragment.md" boilerplate var-header="**`A-JavaFx`: JavaFx**" var-tag="optional" var-fragment="extensions.mbdf#A-JavaFx" />
</box>


<!--

<br><br>



<include src="dukeFragment.md" boilerplate var-header="**`A-Jar`: JAR file**" var-fragment="extensions.mbdf#A-Jar" />

<include src="dukeFragment.md" boilerplate var-header="**`A-CodingStandard`: Coding Standard**" var-fragment="extensions.mbdf#A-CodingStandard" />

<include src="dukeFragment.md" boilerplate var-header="**`A-Gradle`: Gradle**" var-fragment="extensions.mbdf#A-Gradle" />
<include src="dukeFragment.md" boilerplate var-header="**`A-CheckStyle`: CheckStyle**" var-tag="optional" var-fragment="extensions.mbdf#A-CheckStyle" />


<include src="dukeFragment.md" boilerplate var-header="**`A-Assertions`**" var-fragment="extensions.mbdf#A-Assertions" />
<include src="dukeFragment.md" boilerplate var-header="**`A-CodeQuality`**" var-fragment="extensions.mbdf#A-CodeQuality" />
<include src="dukeFragment.md" boilerplate var-header="**`A-Lambdas`**" var-tag="optional" var-fragment="extensions.mbdf#A-Lambdas" />
<include src="dukeFragment.md" boilerplate var-header="**`A-Streams`**" var-tag="optional" var-fragment="extensions.mbdf#A-Streams" />
<include src="dukeFragment.md" boilerplate var-header="**`A-Travis`: Travis**" var-tag="optional" var-fragment="extensions.mbdf#A-Travis" />
<include src="dukeFragment.md" boilerplate var-header="**`A-UserGuide`: User Guide**" var-fragment="extensions.mbdf#A-UserGuide" />
<include src="dukeFragment.md" boilerplate var-header="**`A-Release`: Release**" var-fragment="extensions.mbdf#A-Release" />

</box>

-->




<br>

</div>
</div>
{% endmacro %}

{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("project-w04-mid-v10", show_main_text) }}
