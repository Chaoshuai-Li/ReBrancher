# ReBrancher

---

[![Watch the video](https://img.@*-*@.com/vi/T-D1KVIuvjA/maxresdefault.jpg)](https://youtu.be/T-D1KVIuvjA)

**The conditional branching statements commonly used by developers is a runtime decision-making construct that can deal with multiple conditional expressions and the collection of corresponding execution statements, including if-else statements and switch statements.**

**However, they are becoming harder to review with repeated execution branches and deeply nested conditional clauses as the software life cycle evolves. With JDK 14 officially allowing removing default the fall-through semantic and supporting switch expressions, refactoring the existing conditional branching statements would be extremely valuable to developers. Existing efforts have not focused on these refactorings, which are obviously time-consuming and omission-prone to do manually.**

**We present an automated refactoring approach called ReBrancher that assists developers in refactoring existing conditional branching statements. ReBrancher, based on control flow analysis, data dependency analysis, and the intermediate representation of static analysis, builds the automaton for each conditional branching statement to analyze the branch pattern for detecting repeated execution branches and optimizing nested if-else statements. We designed fall-through analysis and switch pattern analysis to remove redundant fall-through semantics and to refactor conditional branching statements into switch expressions which make the code cleaner and safer.**
