{% from "schedule/index.md" import show_week_pagetop with context%}
{{ show_week_pagetop(4, "tutorial") }}

**Suggested tutorial activities**

### Practice GitHub PR workflow

- Fork the [sample repo for PR practise](https://github.com/nusCS2113-AY1920S1/samplerepo-things) and clone it to your laptop.
- Follow instructions from your tutor to complete this exercise.

<br>

### Polymorphism

<box>
Consider the two scenarios below:

1. You are building the back-end software for an online library that loans e-magazines, music and movies. You decide to implement each of these items as classes.
As you can expect, there are a few common aspects of loaning e-magazine, music or movies. Identify these common aspects (attributes and methods).


2. You are working for a company that specialize in data persistence and storage for software. The current version of your library allows the users to store data in various formats.
E.g., into a SQL database for warehousing and analysis, excel sheets for managers and csv files  for ease of data transportation. Each part of the client software can use some aspects of your library. Your task is to provide a consistent view of the library features to the users. 
</box>

- In both the scenarios above, discuss with your peers what mechanism you would use to achieve the objective? 
- Explain your solution to your peers using a class diagram.

### Regression testing

- Show to your tutor how you achieved regression testing of Duke.

<!--

<tip-box type="important"> 

At this point we would like to ensure that **you are able to create branch-based PRs without accidentally mixing commits** between PRs (a common mistake)
Therefore, we **strongly encourage you to learn the topic: `W4.5 -> Pull requests` before attempting other exercises**.

</tip-box>

    
<tip-box type="important"> 

There are no tutorials this week due to CNY. <br>
However, you are advised to set a time and meet with your team to complete the tasks for **mid-v1.0** and start working towards completing the first draft of the user guide.

</tip-box>

# Suggested exercises

- The following exercises allow you to get used to larger codebase of Addressbook-Level2 and Addressbook-Level3 while at the same time introducing you to various OOP fundamentals.
  - You may feel intimidated by the number of exercises. However, please note that ==it is **not** mandatory to do all of these exercises==.
  - If you are comfortable with the topic you can skip the exercise.
  - You won't be graded for these exercises, but your tutors will provide feedback on your submissions.
- Please submit clean pull-requests to the respective upstream repositories (==take care to submit PRs to nusCS2113-AY1819S2/addressbook-levelX and not the se-edu upstream repo==) before the tutorial.
- During the tutorial, show to your tutor the evidence of learning the topic(s) and participate in relevant discussions.

<br>

<br>


## OOP Basics

<tip-box>

For the following exercises:

**Submission**: Create a PR against [Addressbook-Level2]({{module_org}}/addressbook-level2).  ==Try to make a _clean_ PR== (i.e. free of unrelated code modifications).

==Remember to use team ID== (e.g. _M11-2_) in your PR title.

<panel src="../../admin/appendixE-gitHub.md#tutorial-pr-instructions" header="%%Admin {{ icon_embedding }} Appendix E: Using GitHub → Submitting Pull Requests as evidence of learning a topic%%" />

</tip-box>


<br>

#### [W2.6c] Implement a class

%%==Note==: In the above heading `[W2.6c]` is the id of the exercise  to be used in the PR title (applicable to all exercises)%%

Relevant exercise in Addressbook-Level2: [[Implement a class]({{module_org}}/addressbook-level2/blob/master/docs/LearningOutcomes.adoc#implement-a-class-code-lo-implementclass-code)]


#### [W2.6e] Encapsulation

Relevant exercise in Addressbook-Level2: [[Encapsulation]({{module_org}}/addressbook-level2/blob/master/docs/LearningOutcomes.adoc#apply-encapsulation-code-lo-encapsulation-code)]


#### [W2.6h] Class level members

Relevant exercise in Addressbook-Level2: [[Class-level members]({{module_org}}/addressbook-level2/blob/master/docs/LearningOutcomes.adoc#use-class-level-members-code-lo-classlevel-code)]

#### [W3.1d] Inheritance

Relevant exercise in Addressbook-Level2: [[Inheritance - for code reuse]({{module_org}}/addressbook-level2/blob/master/docs/LearningOutcomes.adoc#use-inheritance-to-achieve-code-reuse-code-lo-inheritance-code)]

<br>

<br>

## OOP Intermediate

<tip-box>


For the following exercises:

**Submission**: Create a PR against [Addressbook-Level3]({{module_org}}/addressbook-level3).  ==Try to make a _clean_ PR== (i.e. free of unrelated code modifications).

==Remember to use team ID== (e.g. _M11-2_) in your PR title. 

<panel src="../../admin/appendixE-gitHub.md#tutorial-pr-instructions" header="%%Admin {{ icon_embedding }} Appendix E: Using GitHub → Submitting Pull Requests as evidence of learning a topic%%" />

</tip-box>


<br>

#### [W4.1c] Polymorphism

Relevant exercise in Addressbook-Level3: [[Using Polymorphism]({{module_org}}/addressbook-level3/blob/master/docs/LearningOutcomes.adoc#use-polymorphism-code-lo-polymorphism-code)]


#### [W4.1d] Abstract class/method

Relevant exercise in Addressbook-Level3: [[Abstract classes/methods]({{module_org}}/addressbook-level3/blob/master/docs/LearningOutcomes.adoc#use-abstract-classes-methods-code-lo-abstract-code)]

#### [W41.g] Interfaces

Relevant exercise in Addressbook-Level3: [[Interfaces]({{module_org}}/addressbook-level3/blob/master/docs/LearningOutcomes.adoc#use-interfaces-code-lo-interfaces-code)]


<br>

<br>


## Requirements analysis

<tip-box>

For the following exercises:

**Submission**: Create a PR against [Addressbook-Level3]({{module_org}}/addressbook-level3).  ==Try to make a _clean_ PR== (i.e. free of unrelated code modifications).

==Remember to use team ID== (e.g. _M11-2_) in your PR title. 

<panel src="../../admin/appendixE-gitHub.md#tutorial-pr-instructions" header="%%Admin {{ icon_embedding }} Appendix E: Using GitHub → Submitting Pull Requests as evidence of learning a topic%%" />

</tip-box>

==Note: If you have completed recording user stores, use cases and non-functional requirements for your project, it is not necessary to do the exercises below.==

Show to your tutor relevant items from your project to get feedback.

 <br>

 
#### [W4.2b] Non-functional requirements

Relevant exercise in Addressbook-Level3: [[User cases]({{module_org}}/addressbook-level3/blob/master/docs/LearningOutcomes.adoc#use-non-functional-requirements-code-lo-nfr-code)]

#### [W4.4a] User stories

Relevant exercise in Addressbook-Level3: [[User stories]({{module_org}}/addressbook-level3/blob/master/docs/LearningOutcomes.adoc#utilize-user-stories-code-lo-userstories-code)]


#### [W4.4d] Use cases

Relevant exercise in Addressbook-Level3: [[User cases]({{module_org}}/addressbook-level3/blob/master/docs/LearningOutcomes.adoc#utilize-use-cases-code-lo-usecases-code)]

-->
