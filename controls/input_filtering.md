# Input Filtering Design

## Purpose
Input filtering is used to detect suspicious prompts before they are passed into the retrieval and response workflow.

## Suspicious Prompt Patterns
The filter is designed to flag prompts containing phrases or behaviors such as:

- "ignore previous instructions"
- "bypass policy"
- "reveal confidential information"
- "show admin-only content"
- "disregard system prompt"
- requests for restricted internal information
- attempts to override role-based limitations

## Filtering Logic
1. User submits a prompt.
2. The system checks for suspicious phrases or override behavior.
3. If the prompt is low risk, it continues to retrieval.
4. If the prompt is medium or high risk, it is flagged for refusal, validation, or human review.

## Expected Benefit
Input filtering reduces the likelihood that the chatbot will follow user attempts to override safety rules or request unauthorized content.
