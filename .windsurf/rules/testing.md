---
trigger: model_decision
description: Always attach when Implementing Code (Act/Code MODE)
globs: 
---
---
description: Include these rules while IMPLEMENTATION/Coding.
globs: 
alwaysApply: true
---

[Step: 3] <MAKE CHANGES>

1. Document Current State in files specified by @memory.mdc  
- What’s currently working?  
- What’s the current error/issue?  
- Which files will be affected?

2. Plan Single Logical Change at a Time

<INCREMENTAL ROLLOUTS>
- One logical feature at a time  
- But fully resolve this one change by accommodating appropriate changes in other parts of the code.  
- Adjust all existing dependencies and issues created by this change.  
- architecture_preservation: Ensure that all new code integrates seamlessly with existing project structure and architecture before committing changes. Do not make changes that disrupt existing code organization or files.
</INCREMENTAL ROLLOUTS>

3. Simulation Testing

<SIMULATION ANALYSIS>
- Simulate user interactions and behaviors by performing dry runs, trace calls, or other appropriate methods to rigorously analyze the impact of proposed changes on both expected and edge-case scenarios.  
- Generate feedback on all potential side effects.
</SIMULATION ANALYSIS>

<SIMULATION VALIDATION>
- Do not propose a change unless the simulation passes and verifies that all existing functionality is preserved, and if a simulation breaks, provide fixes immediately before proceeding.
</SIMULATION VALIDATION>

- If Simulation Testing Passes, do the actual implementation.

[Step: 4] Perform <TESTING>

[Step: 5] LOOP 1-4 and implement all changes  
- Incorporate all the changes systematically, one by one.  
- Verify the changes and test them one by one.

[Step: 6] Optimize the implemented codes  
- Optimize the implemented code, after all changes are tested and verified.

</SYSTEMATIC CODE PROTOCOL>

<REFERENCE>
- Reference relevant documentation and best practices  
- Use <WEB USE> if needed to refer to documentation or best practices
</REFERENCE>

# TESTING (Always write TEST after IMPLEMENTATION) [ACT/Code MODE]
<TESTING>

<DEPENDENCY BASED TESTING>  
Create unit tests for any new functionality. Run all tests from the <ANALYZE CODE> to confirm that existing behavior is still as expected.  
</DEPENDENCY BASED TESTING>

<NO BREAKAGE ASSERTION>  
After you propose a change, run the tests yourself, and verify that it passes. Do not rely on me to do this, and be certain that my code will not be broken.  
</NO BREAKAGE ASSERTION>

1. Write test logic in separate files than the code implementation for the functionality to keep the code clean and maintainable

<TEST PLAN>
- Think of sufficiently exhaustive test plans for the functionalities added/updated against the requirements and desired outcomes.  
- Define comprehensive test scenarios covering edge cases  
- Specify appropriate validation methods for the project's stack  
- Suggest monitoring approaches to verify the solution's effectiveness  
- Consider potential regressions and how to prevent them  
</TEST PLAN>

2. Write test code for ANY added critical functionality ALWAYS. For initial test generation use <DEPENDENCY BASED TESTING> and <NO BREAKAGE ASSERTION>. Then use <TEST PLAN> to write code for extensive testing.

3. Document testing as specified in @memory.mdc

After every code implementation/change ALWAYS do 2 things:  
b. Update the documentation in `docs/` and `tasks/`.
</TESTING>