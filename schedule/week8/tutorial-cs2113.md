{% from "schedule/index.md" import show_week_pagetop with context%}
{{ show_week_pagetop(8, "tutorial") }}

## Questions to discuss during tutorial:

<panel header="{{icon_Q }} Questions">
<question>

1. Explain what Gradle is. How is it used in your project?
1. Explain what Travis is. How is it used in your project?
1. Which integration approach is used by the project?
1. What’s the difference between _buffers_ and _padding/inflating_ estimates?

</question>
</panel>


## Suggested tutorial activities

<panel header="{{icon_Q }} Model the relation between the students and tasks">
<question>

A course in the university can have a number tasks which can be assignments or tests. 
Some assignments are compulsory. <br>
When a student attempts a task, a grade and an optional feedback is given.

</question>
</panel>


<include src="../../book/modeling/modelingStructures/classDiagramsIntermediate/q-explainClassDiagramNotation.md" />

<include src="../../book/modeling/modelingStructures/classDiagramsIntermediate/q-drawClassDiagramForItemEtc.md" />

<include src="../../book/modeling/modelingBehaviors/sequenceDiagramsIntermediate/q-essay-expainParserFactory.md" />

<include src="../../book/modeling/modelingBehaviors/sequenceDiagramsIntermediate/q-drawPrintQuoteSd.md" />






<!--
<panel header="{{ icon_Q }} Architecture">
<question>

1. Which architecture styles are used by AB-4?
1. What is an API? How is it used in AB-4?

</question>
</panel>
-->