{% from "schedule/index.md" import show_week_pagetop with context%}
{{ show_week_pagetop(8, "tutorial") }}

## Questions to discuss in the tutorial

<panel header="{{icon_Q }} Question set 1">
<question>

1. What is abstraction? How is it used in the project?
1. What is coupling?
   1. `Foo` depends on `Bar` if …?
   1. Give examples of different ways how a class `Foo` can be coupled to `Bar`
1. What is cohesion?
1. How does cohesion relates to coupling?

</question>
</panel>


<panel header="{{icon_Q }} Question set 2">
<question>

1. What is the Principle of SoC?
1. How does SoC relate to coupling and cohesion?
1. What is SRP?
1. How does SRP relate to SoC?

</question>
</panel>

<panel header="{{icon_Q }} Question set 3">
<question>

1. What is OCP?
1. Explain several different ways of achieving OCP
1. Does the project follow OCP? E.g. Can we add a new command or a new storage type without modifying existing code too much?

</question>
</panel>

<panel header="{{icon_Q }} Model the relation between the students and tasks">
<question>

A course in the university can have a number tasks which can be assignments or tests. 
Some assignments are compulsory. <br>
When a student attempts a task, a grade and an optional feedback is given.

</question>
</panel>

<br>

## Suggested tutorial activities



<include src="../../book/modeling/modelingStructures/classDiagramsIntermediate/q-explainClassDiagramNotation.md" />

<include src="../../book/modeling/modelingStructures/classDiagramsIntermediate/q-drawClassDiagramForItemEtc.md" />

<include src="../../book/modeling/modelingBehaviors/sequenceDiagramsIntermediate/q-essay-expainParserFactory.md" />







<!--
<panel header="{{ icon_Q }} Architecture">
<question>

1. Which architecture styles are used by AB-4?
1. What is an API? How is it used in AB-4?

</question>
</panel>
-->