# AI Workflow Comparison

## Overview

For this exercise, I completed the same task using two different AI-assisted workflows to compare the quality of the generated results.

In Round 1, I used a very simple prompt with minimal instructions and accepted the generated output with little guidance. In Round 2, I used a much more structured workflow by providing clear requirements, expected behavior, project constraints, verification steps, and project-specific rules. Each version was maintained in its own Git branch for comparison.

## Round 1 – Vague Prompt

The first approach required very little effort to start because the prompt was short. However, the generated result lacked detail and required more manual review. Some implementation decisions were made without enough context, and important considerations such as accessibility, validation consistency, testing, and edge cases were either missing or only partially addressed.

Reviewing the generated output took longer because I had to inspect the code carefully and determine whether the implementation matched the expected behavior.

## Round 2 – Detailed Prompt

The second approach used a detailed prompt with explicit project requirements and verification instructions. The AI had clearer guidance about what was expected before generating code.

Compared to the first version, the generated work was more structured and easier to review. Accessibility requirements, validation expectations, testing, and project-specific rules were considered from the beginning. The review process was faster because fewer assumptions had to be corrected manually.

## Comparison

The detailed workflow produced a better overall result. Although writing the prompt required more time, it reduced the amount of manual review needed afterward. The generated output was easier to understand, more consistent, and better aligned with project expectations.

One AI mistake I identified during review was that the initial implementation relied on assumptions instead of explicit requirements. Without sufficient guidance, some expected behaviors and validation details were incomplete. Providing clearer instructions in the second workflow significantly reduced these issues.

## Conclusion

This exercise demonstrated that effective AI-assisted development depends on the quality of the instructions provided to the model. A structured workflow that includes planning, clear constraints, verification, and review produces more reliable and maintainable results than relying on a single vague prompt.