# ReBrancher

---

**The conditional branching statements commonly used by developers is a runtime decision-making construct that can deal with multiple conditional expressions and the collection of corresponding execution statements, including if-else statements and switch statements.**

**However, they are becoming harder to review with repeated execution branches and deeply nested conditional clauses as the software life cycle evolves. With JDK 14 officially allowing removing default the fall-through semantic and supporting switch expressions, refactoring the existing conditional branching statements would be extremely valuable to developers. Existing efforts have not focused on these refactorings, which are obviously time-consuming and omission-prone to do manually.**

**We present an automated refactoring approach called ReBrancher that assists developers in refactoring existing conditional branching statements. ReBrancher, based on control flow analysis, data dependency analysis, and the intermediate representation of static analysis, builds the automaton for each conditional branching statement to analyze the branch pattern for detecting repeated execution branches and optimizing nested if-else statements. We designed fall-through analysis and switch pattern analysis to remove redundant fall-through semantics and to refactor conditional branching statements into switch expressions which make the code cleaner and safer.**

The repository contains packaged Eclipse plugins with the zip file type.

Steps for importing to Eclipse IDE. 

"Open Eclipse IDE" -> "Help" -> "Install New Software" -> "Add" -> "Archive" -> Select the Zip file in your path -> "Select All" -> "Next" -> Accept and Finish

However, according to feedback from others, the following __"The chosen file is not enable"__ exists when selecting a project to refactor after importing the plugin .

The reasons for this are as follows: 1) The static analysis tool is not robust enough in terms of environment configuration requirements for refactoring scenarios involving switch expression refactoring for JDK14 onwards. 2) The graphical tool Graphviz is prone to crashes and can easily lead to the unavailability of plugins when encapsulated into plugins.

We are working on this issue, so please understand and stay tuned.

We are recording ReBrancher available videos locally to show it

Below are the available videos and repositories for our previous work on __ReSwitcher__, which you can sample [here](https://github.com/Chaoshuai-Li/ReSwitcher-Plugin).

[![Watch the video](https://github.com/Chaoshuai-Li/ReSwitcher/blob/main/reswitcher.png)](https://www.youtube.com/watch?v=utdHUQjI1Vo)
