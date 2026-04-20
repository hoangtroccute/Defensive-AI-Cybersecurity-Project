# Checkpoint 3 — Defensive Controls and Validation Progress

## Project Title
Defending an Internal RAG Chatbot Against Prompt Injection Attacks

## System Context
This project studies an internal Retrieval-Augmented Generation (RAG) chatbot used by employees to ask questions about HR, IT, and internal policy documents. In the baseline system, the chatbot could retrieve internal documents and answer questions, but it did not yet include strong protections against prompt injection, insecure retrieval, unauthorized disclosure, or weak output review.

Checkpoint 3 focuses on moving beyond analysis into defensive action. At this stage, the group selected practical controls, documented why they were chosen, and evaluated how they improve security compared to the baseline.

## Controls Selected
The team selected the following defensive controls for evaluation:

1. **Document trust labeling**  
   Documents are categorized by trust level so the system can prefer approved internal sources and avoid low-trust content.

2. **Input filtering**  
   Suspicious prompts are flagged when users attempt to override rules, request restricted information, or manipulate the chatbot.

3. **Retrieval restrictions**  
   The retriever is limited to approved document categories and excludes content that should not be used in general employee responses.

4. **Access-aware retrieval**  
   Document access is matched to user role so employees only receive content they are allowed to see.

5. **Output validation**  
   Responses are checked before display to reduce unsafe, sensitive, or policy-violating outputs.

6. **Logging improvements**  
   Prompt attempts, retrieval choices, and final outputs are recorded more clearly for review and traceability.

7. **Human review for high-risk cases**  
   Requests involving restricted data or uncertain outputs are escalated for manual review instead of being answered automatically.

## Why These Controls Were Selected
These controls were selected because they directly address the biggest risks identified in Checkpoint 2:

- prompt injection in retrieved documents
- direct prompt manipulation
- unauthorized information disclosure
- insecure retrieval
- weak output validation
- weak logging and monitoring

The team chose controls that are realistic for a one-month defensive project and can be clearly compared against the baseline system. Rather than trying to redesign the entire chatbot, the group focused on protections that are practical, explainable, and easy to evaluate through test cases.

## Validation Progress
The selected controls were evaluated against baseline prompt and retrieval scenarios. Results show reduced unsafe behavior, improved handling of suspicious prompts, lower risk of unauthorized disclosure, and better traceability through improved logging.

## Deliverables Included in This Checkpoint
- control implementation/evaluation summary
- evidence of defensive work
- validation evidence
- updated risk register
- draft outline of final report
