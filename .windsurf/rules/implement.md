---
trigger: model_decision
description: Always attach when Implementing Code (Act/Code MODE)
---

---
description: Include these rules while IMPLEMENTATION/Coding.
globs: 
alwaysApply: true
---
# IMPLEMENTATION (ACT MODE/Code MODE)

Before every code implementation/change ALWAYS do 2 things:
a. Read and understand the documentation in `docs/` and `tasks/`
b. Use context7, fecth and serper-search-server mcp to get documentation how to implement the code.

## Programming Principles

<PROGRAMMING PRINCIPLES>
- algorithm_efficiency: use the most efficient algorithms and data structures
- modularity: write modular code, break complex logic into smaller atomic parts. Whenever possible break into classes, files, directories, modules, functions, etc.
- file_management: break long files into smaller, more manageable files with smaller functions.
- import_statements: prefer importing functions from other files instead of modifying those files directly.
- file_organization: organize files into directories and folders.
- reuse: prefer to reuse existing code instead of writing it from scratch.
- code_preservation: Preserve What Works. Don't modify working components without necessity.
- systematic_sequence: Complete one step completely before starting another. Keep systematic sequence of functionalities.
- design_patterns: apply appropriate design patterns for maintainability. Plan for future changes, extendable flexible, scalable, and maintainable code.
- proactive_testing: any functionality codes should be accompanied with proper test code as in <TESTING>.
</PROGRAMMING PRINCIPLES>

## Systematic Code Protocol

<SYSTEMATIC CODE PROTOCOL>

[Step: 1] <ANALYZE CODE>

<DEPENDENCY ANALYSIS>
- Which components will be affected?
- What dependencies exist?
- Is this local or does it affect core logic?
- Which functionalities will be affected and how?
- What cascading effects will this change have?
</DEPENDENCY ANALYSIS>

<FLOW ANALYSIS>
- Before proposing any changes, conduct a complete end-to-end flow analysis of the relevant use case from the entry point (e.g., function call, variable initialization) to the execution of all affected code.
- Track the flow of data and logic throughout all components involved to understand its full scope.
</FLOW ANALYSIS>

- Document these dependencies thoroughly, including the specific usage of functions or logic in files specified by @memory.mdc

[Step: 2] <PLAN CODE>

- If needed initiate <CLARIFICATION> process.
- Use <STEP BY STEP REASONING> to Outline a detailed plan including component dependencies, architectural considerations before coding. Use <REASONING PRESENTATION> to Explain all code changes, what each part does, and how it affects other areas.

<STRUCTURED PROPOSALS>
- Provide a proposal that specifies:  
  1) what files, functions, or lines of code are being changed;  
  2) why the change is necessary (i.e. bug fix, improvement or new feature);  
  3) all of the directly impacted modules or files;  
  4) potential side effects;  
  5) a detailed explanation of any tradeoffs.
</STRUCTURED PROPOSALS>
</PLAN CODE>