{% from "schedule/index.md" import show_week_pagetop with context%}
{{ show_week_pagetop(9, "tutorial") }}

## Questions to discuss during tutorial:

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


<panel header="{{icon_Q }} Question set 4">
<question>

1. What is _unit/integration/system/acceptance_ testing?
1. What’s the difference between _unit testing_ and _integration testing_?
1. What’s the difference between _system testing_ and _acceptance testing_?
1. Which integration approach is used in your project?

</question>
</panel>




## Suggested tutorial activity

<include src="../../book/modeling/modelingStructures/classDiagramsBasic/q-essay-explainClassDiagram.md" />

<include src="../../book/uml/classDiagrams/combine/basic/q-essay-objectDiagramsForClassDiagram.md" />

 