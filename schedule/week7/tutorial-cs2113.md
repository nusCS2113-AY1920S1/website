{% from "schedule/index.md" import show_week_pagetop with context%}
{{ show_week_pagetop(7, "tutorial") }}

# Suggested tutorial activities

### Project management - Issue tracker

- Setup the issue tracker as per the [instructions]({{ module_website }}/admin/appendixE-gitHub.html#issue-tracker-setup), if you haven't done yet.
- Record all your user stories as issues.
- Try to identify `type.Epic` issues from corresponding `type.Story`.
- Assign priority labels to all the issues.
- Split the `type.Story` issues to `type.Task`.

### Project management - Scheduling

- Create milestones: `v1.1`, `v1.2`, `v1.3`, `v1.4`, and set the deadline to be the day before your tutorial in weeks  7, 9, 11 and 13.
- At minimum, assign some `type.Epic` or `type.Story` issues to each milestone.
  - (Preferred) assign all `type.Story`, `type.Epic` and `type.Task` issues to each milestone.
- Assign at least one owner to each `type.Story` and `type.Task` to all the issues in `v1.2`. 

### Architecture


<question>

1. Which architecture styles are using in your project?
1. Identify the components in your product and draw the architecture diagram.
1. What is an API? Identify the API that your product (more specifically its components) provides.
1. What is the design approach you are following in your project?

</question>
    