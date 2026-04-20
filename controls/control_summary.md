# Control Summary

## Selected Defensive Controls

| Control | Purpose | Threat Reduced |
|---|---|---|
| Document trust labeling | Separate trusted from low-trust retrieval sources | Prompt injection, insecure retrieval |
| Input filtering | Flag suspicious user prompts | Direct prompt manipulation |
| Retrieval restrictions | Limit which documents can enter context | Insecure retrieval |
| Access-aware retrieval | Match document access to user role | Unauthorized disclosure |
| Output validation | Check for unsafe or sensitive responses | Unauthorized disclosure, unsafe output |
| Logging improvements | Record prompts, retrieval, and outputs | Weak logging and monitoring |
| Human review for high-risk cases | Add manual review for sensitive or uncertain requests | High-impact unsafe responses |

## Summary
These controls were chosen because they directly address the highest-priority risks found during baseline analysis. Together they strengthen the chatbot against prompt injection, reduce disclosure risk, and improve review capability.
