# Retrieval Restrictions and Hardening

## Purpose
Retrieval restrictions are used to control which documents can enter the model context.

## Retrieval Hardening Measures
- only approved internal sources are eligible for retrieval
- low-trust or unreviewed files are excluded
- restricted documents are separated from general employee materials
- role-aware filtering is applied before retrieved content is passed to the model

## Why This Matters
Because retrieved content directly influences the LLM response, unsafe or untrusted documents increase the risk of prompt injection and inaccurate output.

## Expected Benefit
Retrieval hardening reduces the chance that malicious, irrelevant, or restricted content will shape the chatbot response.
