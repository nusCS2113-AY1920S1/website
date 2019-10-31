{% from "schedule/index.md" import show_week_pagetop with context%}
{{ show_week_pagetop(11, "tutorial") }}

# Suggested tutorial activities:

### Demo
**Two members together do a quick demo of your v1.3 using the jar file**

### Suggested tutorial activity

**Test case design**

==Whole team: do this question together, using the whiteboard==

<div class="indented">
  <include src="../../book/testCaseDesign/combiningTestInputs/mix/q-testCasesForConsumeMethod.md" />
</div>
<br>

### Questions

==Divide the following questions among team members and get ready to answer them.==

**Q1**

1. What is _Liskov Substitution Principle_?<br>
   Give an example from the project where LSP is followed and explain how to change the code to break LSP.
1. Explain how _Law of Demeter_ affects coupling<br>
   a. Add a line to this code that violates LoD
   ```java
   void foo(P p){
       //...
   }
   ```
1. Give an example in the project code that violates the _Law of Demeter_.

**Q2.** Design patterns.
1. When do you use _MVC_ pattern?
1. When do you use the Singleton pattern, Command pattern? 
<!--
1. When do you use the _Facade_ pattern; _Observer_ pattern? Do we have the Observer pattern in AB4?
-->
**Q3.** Process models

1. Distinguish between _sequential_ and _iterative_ processes. Which one are we using in the project?
1. Distinguish between _breadth-first_ and _depth-first_ iterative processes using your project as an example.
1. Describe how _agile process models_ differ from traditional process models.

**Q4.** XP and Scrum

(Divide XP and Scrum between the two teams for the following activity, if there is enough time left.)

* Each team use the Web to find about 5 distinguishing features of the process model.
  * Some interesting [SCRUM concepts](https://www.scrum.org/resources/what-is-scrum): Product backlog, scrum board, story points, burndown charts, scrum master, product owner
  * XP rules are described at [http://www.extremeprogramming.org/rules.html](http://www.extremeprogramming.org/rules.html)

* Relate those features to your project. %%i.e. are they applicable? are you doing something similar?%%
