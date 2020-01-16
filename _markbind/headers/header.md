{% from "schedule/index.md" import weeks, current_weeks with context %}
<header>
<div class="w-100 p-1 bg-warning text-center"><md>**This site is from a past semester! The current version is [here](http://www.comp.nus.edu.sg/~{{ module | lower }}).**</md></div>
<navbar placement="top">
  <a slot="brand" href="{{baseUrl}}/index.html" title="Home" class="navbar-brand">{{ module_pair }} <small>{{ period }}</small></a>
  <dropdown text="Schedule" class="nav-link">
{% for week in weeks %}
<li><a href="{{ baseUrl }}/schedule/week{{ week.num }}/index.html" class="dropdown-item"> <md>**Week {{ week.num }}** [{{ week.day }}] {% if current_weeks[0] == week.num %} :fas-arrow-circle-left:{% endif %}</md></a></li>
{% endfor %}
  </dropdown>
  <li><a href="{{baseUrl}}/se-book-adapted/index.html" class="nav-link"><md>**Textbook**</md></a></li>
  <li><a href="{{baseUrl}}/admin/index.html" class="nav-link"><md>**Admin Info**</md></a></li>
  <dropdown text="Links" class="nav-link">
    <li><a href="{{bugs_link}}" target="_blank" class="dropdown-item"><md>:fas-bug:</md> Report Bugs</a></li>
    <li><a href="{{slack_team}}" target="_blank" class="dropdown-item"><md>:fab-slack-hash:</md> Slack</a></li>
    <li><a href="{{forum_link}}" target="_blank" class="dropdown-item"><md>:fas-comment:</md> Forum</a></li>
    <li><a href="{{baseUrl}}/admin/project-overview.html" class="dropdown-item">{{ icon_project }} Project Info</a></li>
    <li><a href="{{ baseUrl }}/admin/instructors.html" class="dropdown-item"><md>:fas-user-tie:</md> Instructors</a></li>
    <li><a href="{{ivle_announcements}}" target="_blank" class="dropdown-item"><md>:glyphicon-bullhorn:</md> Announcements</a></li>
    <li><a href="{{ivle_files}}" target="_blank" class="dropdown-item"><md>:fas-file-upload:</md> File Submissions</a></li>
    <li><a href="{{baseUrl}}/admin/tutorials.html" target="_blank" class="dropdown-item"><md>:glyphicon-calendar:</md> Tutorial Schedule</a></li>
    <li><a href="https://github.com/nus{{ module | lower }}-{{ semester }}/duke" target="_blank" class="dropdown-item">{{ icon_repo }} Duke </a></li>
    <li><a href="https://nus{{ module | lower }}-{{ semester | lower }}.github.io/phase1-dashboard" target="_blank" class="dropdown-item"><md>:fas-chart-area:</md> Project Phase1 Dashboard</a></li>
    <li><a href="{{java_coding_standard}}" target="_blank" class="dropdown-item"><md>:fas-code:</md> Java Coding Standard</a></li>
    <li><a href="{{module_org}}/samplerepo-things" target="_blank" class="dropdown-item">{{ icon_repo }} samplerepo-things</a></li>
    <li><a href="{{baseUrl}}/admin/projectList.html" class="dropdown-item"><md>:fas-th-list:</md> Projects List</a></li>
    <li><a href="{{baseUrl}}/admin/reposenseConfigTemplates.html" class="dropdown-item"><md>:fas-th-list:</md> config.json templates for Reposense</a></li>
    <li><a href="https://github.com/nus{{ module | lower }}-{{ semester }}/PersonalAssistant-Duke" target="_blank" class="dropdown-item">{{ icon_repo }} PersonalAssistant-Duke </a></li>
    <li><a href="https://nus{{ module | lower }}-{{ semester | lower }}.github.io/dashboard" target="_blank" class="dropdown-item"><md>:fas-chart-area:</md> Project Phase2 Dashboard </a></li>
    <li><a href="https://github.com/nus{{ module | lower }}-{{ semester }}/addressbook-level3" target="_blank" class="dropdown-item">{{ icon_repo }} Reference project - Addressbook </a></li>
    <li><a href="https://repl.it/classroom/invite/cuFCDgh" target="_blank" class="dropdown-item"><md>:glyphicon-blackboard:</md> Repl.it classroom</a></li>
  </dropdown>
  <li slot="right" class="nav-link">
    <form class="navbar-form">
      <searchbar :data="searchData" placeholder="Search" :on-hit="searchCallback" menu-align-right ></searchbar>
    </form>
  </li>
</navbar>
</header>
