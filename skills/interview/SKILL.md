---
name: interview
description: Interview the user in a thorough and detailed manner about a prompt to gather every single piece of information needed to craft a production grade implementation plan covering everything from simple facts to most complex edge cases.
---

# interview

Interview the user in a thorough and detailed manner about a prompt to gather every single piece of information needed to craft a production grade implementation plan covering everything from simple facts to most complex edge cases, the interview is conducted in a round by round manner each round presents all the possible questions with the current knowledge and understanding and builds upon the previous rounds until the goal is reached.

## Rules

1. **A round of interview is not complete and the next round can not start untill all the questions in that round are resolved.**
2. **Every question is rendered from `assets/question-template.md`.** Ids are sequential and never reused; each round continues the sequence.
3. **A question is resolved only by a concrete, unambiguous user answer.** "I don't know", hand-waving, or partial answers do not count as resolved.

## Workflow

1. Explore the codebase
   - Explore and study the codebase and gather all the needed information to conduct the interview.

2. If validation fails:
   - Research (Skip if you already have the latest information and necessary understanding of all the main concepts of the matter)

   - Validate based on the current context and understanding, if every piece of information and detail is gathered to fulfill the goal of the skill, this loop ends here and the workflow can be resumed to the next step.

   - Ask the batch (start a round)
     - Ask as many questions as possible based on the current context and information in possession; each round based on the user's answers to the previous questions the context is extended.
     - Present all questions of the batch at once, each rendered from `assets/question-template.md`.

   - Evaluate the answers and if some questions of the batch are not properly answered or answered at all, keep asking them again until a reliable answer is provided and agreed upon.

3. Record the context in a document
   - Use the `assets/interview.md` template, extract and record the required information in the template, from the context.
   - Store the result document in the `.hll/interviews` directory in the project root (create if doesn't exist).
   - Use this naming convention for the document name: `interview-*.md`, the asterisk is a sequential number starting from one and must be derived from the contents of the `.hll/interviews` directory while creating a new document.
