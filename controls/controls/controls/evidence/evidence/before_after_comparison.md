# Before and After Comparison

## Baseline Condition
At baseline, the chatbot could answer employee questions using retrieved internal documents, but it did not yet include strong prompt injection defenses, trust labeling, access-aware retrieval, or output validation. Logging existed only at a limited level.

## Improved Condition
After defensive controls were added, the chatbot workflow included:
- document trust labeling
- input filtering
- retrieval restrictions
- access-aware retrieval
- output validation
- improved logging
- human review for high-risk requests

## Summary of Change
The improved design is more resistant to prompt injection, more careful about restricted information, and easier to review than the baseline model.
