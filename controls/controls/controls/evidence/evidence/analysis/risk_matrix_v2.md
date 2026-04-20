# Updated Risk Matrix

| Threat | Baseline Risk | Updated Risk | Reason for Change |
|---|---|---|---|
| Prompt injection in retrieved documents | Critical | High | Trust labeling, retrieval restrictions, and guardrails reduce success rate |
| Direct user prompt manipulation | High | Medium | Input filtering and refusal logic reduce unsafe compliance |
| Unauthorized disclosure | High | Medium | Access-aware retrieval and output validation lower exposure risk |
| Insecure retrieval | High | Medium | Approved-source restrictions improve document selection |
| Weak output validation | Medium | Low | Added validation layer improves response review |
| Weak logging and monitoring | Medium | Low | Logging design improves traceability and review capability |
| Over-reliance on AI output | Medium | Medium | Review practices help, but human trust risk remains |

## Residual Risk Note
Residual risk still exists because:
- the model may still produce unexpected output
- document labeling could be incomplete
- complex prompts may bypass simple filters
- human reviewers may not always be available
- users may still trust outputs too much without verification
