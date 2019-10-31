{% macro show_main_text() %}
<div id="main">

<div id="title">

</div>
<div id="body">

<p class="lead" style="color: purple"><md>:far-calendar-check: <include src="project-timeline.md#v13-overview" inline /></md></p>



**v1.3 Summary of Milestone**

Milestone | Minimum acceptable performance to consider as 'reached'
--------- | -------------------------------------------------------
{{ icon_individual }} Contributed code to v1.3 | code merged
{{ icon_individual }} Code is RepoSense-compatible | as stated in mid-v1.3
{{ icon_individual }} Generate project portfolio page | extract parts of UG/DG into PPP.
{{ icon_team }} v1.3 jar file released on GitHub | as stated
{{ icon_team }} v1.3 milestone properly wrapped up on GitHub | as stated
{{ icon_team }} Documentation updated to match v1.3 | at least the User Guide and the `README.adoc` is updated

### v1.3 Project Management

* Ensure your code is RepoSense-compatible, <trigger trigger="click" for="modal:v13-reposense">as explained in mid-v1.3</trigger>.

<modal large title="Admin {{ icon_embedding }} Project → v1.3 (extract)" id="modal:v13-reposense">
  <include src="reposenseCompatibility.md" />
</modal>

### v1.3 Product

* As before, move the product towards v2.0.

* {{ icon_important_big_red }} **Do a <tooltip content="resulting in a jar file on GitHub that can be downloaded by potential users">proper product release</tooltip>** [as described in this DevOps page](https://github.com/nusCS2113-AY1920S1/addressbook-level3/blob/master/docs/DevOps.adoc#5-making-a-release). Do some manual tests to ensure the jar file works.

### v1.3 Documentation

<tip-box>

{{ icon_important_big_red }} v1.3 user guide should be updated to match the current version of the product. %%&nbsp;Reason: v1.3 will be subjected to a trial _user testing_ session%%

</tip-box>

* **README page**: Update to look like a real product if you haven't done so already. In particular, ==update the `Ui.png` to match the current product (<trigger trigger="click" for="modal:v13-tipsForProductScreenshot">:bulb: tips</trigger>)==.

<modal large title="Admin → Project Deliverables → Website" id="modal:v13-tipsForProductScreenshot">
  <include src="project-deliverables.md#tips-for-product-screenshot"/>
</modal>
  
* **User Guide**: ==This document will be used by your peer testers==. Update to match the current version. In particular,
  * Clearly indicate which features are not implemented yet %%e.g. tag those features with a `Coming in v2.0`%%.
  * For those features already implemented, ensure their descriptions match the exact behavior of the product %%e.g. replace mockups with actual screenshots%%
 
* **Developer Guide**: As before, update if necessary.
  
* **AboutUs page**: Update to reflect current state of roles and responsibilities.  

* **Product portfolio page**: See below for details.

**Submission**: PDF submitted on LumiNUS.

#### Project Portfolio Page (PPP)
<include src="project-deliverables.md#project-deliverables-ppp"/>

### v1.3 Demo

* Do a quick demo of the main features ==using the jar file==. Objective: demonstrate that the jar file works.


### v1.3 Testing (_aka_ Practical Exam Dry Run)

%%Information updated on 30/10/2019%%  
See info in the panel below:

<br>
{{ embed_topic("project-deliverables.md#project-deliverables-practicalexam-dry-run", "Admin " + icon_embedding + " Project Deliverables → **Practical Exam - Dry Run**", "v13-peDryRun", "1") }}


</div>
</div>
{% endmacro %}

{% from "common/macros.njk" import embed_topic with context %}
{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("project-w11-v13", show_main_text) }}