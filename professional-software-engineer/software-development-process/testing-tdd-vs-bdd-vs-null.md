---
description: >-
  Must-know approaches to develop quality software. Making an app runnable is
  one thing. Ensuring it is doing the right things is equally important. Testing
  is the guardian. Be a responsible developer.
---

# Testing - TDD vs BDD

## TDD - Test-Driven Development \| Short Intro

### **\[Core stakeholders in concern\]** 

Programmers \(or say, Developers\)

###  **\[Core spirit\]** 

**Write tests before writing code.** 

TDD is a **process to write code** through **a short and repeated cycle** called Red-green-refactor.

### \[Execution\] : Red\(Step1\) -&gt; Green\(Step2\) -&gt; Refactor\(Step3\)

**1-1\) Write tests** - List out the expected behaviors of code, in a format of test cases.

**1-2\) Run all tests** - Should be100% fail \(i.e red\) because there is not yet any implementation code.

**2-1\) Write the implementation code** - Make the code work \(i.e. Write only enough code to fulfill the expected behaviors listed in step 1\)

**2-2\) Run all tests** - Should be 100% pass\(i.e. green\) at this time point, to ensure code is doing the right things.

**3-1\) Refactor code** - Make the code elegant \(i.e. maintainable, readable, etc\). 

**3-2\) Run all tests** - Should be 100% pass\(i.e. green\) at this time point, to ensure 3-1 did not break anything completed in 2-1.

### **\[Advantages of TDD\]**

**1\) Executable Documentation** - Save effort writing extra documentation

Tests in TDD become Executable Documentation. 

During traditional development, we often write documentation like a diary to give additional information about our code \(e.g what is the purpose of some code methods\) for future record-trace. The problem is that developers often need extra effort to maintain the documentation because documentation will inevitably get out-dated once there is any update in the code. Documentation is not reliable if no one is actively maintaining it.

With TDD we can solve this problem because the tests themselves become real-time documentation. 





