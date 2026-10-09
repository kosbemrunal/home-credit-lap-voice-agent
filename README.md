# Home Credit LAP Voice Agent

An AI voice-agent assignment project built with Retell AI to conduct preliminary qualification for a Home Credit Loan Against Property (LAP) offer.

## Project objective

The agent contacts an existing customer, verifies identity and availability, presents the LAP offer of up to ₹75,00,000, gathers seven eligibility data points, handles disqualification and loan-transfer cases, and routes eligible customers to a senior loan expert for follow-up.

## Platform

- Voice-agent platform: Retell AI
- Published version: V0
- Conversation instructions: [`system_prompt.txt`](system_prompt.txt)

## Eligibility rules implemented

1. **Property type:** Residential, commercial, and industrial are eligible. Agricultural property is not eligible.
2. **Ownership:** Sole and joint ownership are both eligible.
3. **Original documents:** Original property documents must be available for verification.
4. **Loan amount:** Maximum ₹75,00,000. If a customer requests more, explain the cap and ask whether they want to proceed with the maximum.
5. **Occupation and income mode:** Salaried and self-employed customers may qualify, but income must be received through a bank; cash income is not eligible.
6. **Property market value:** Capture the customer's estimated current market value. Do not invent a minimum threshold.
7. **Tenure:** 3 to 15 years inclusive.

The agent should disqualify promptly when a required criterion fails. If the customer has an existing loan against the property or wants to reduce an existing EMI, the agent should route the case to a loan-transfer specialist. The final expert follow-up should only be stated after all seven eligibility points are answered and the criteria are met.

## Test evidence

Recordings and related evidence are being organized in this Google Drive folder:

[Open call recordings folder](https://drive.google.com/drive/folders/1gSOJqe_zG6RfBOxKqCLo7qzTQW6mXen7?usp=sharing)

Please ensure the folder and each required file are accessible to the reviewer. The test report distinguishes confirmed observations from scenarios that still need transcript verification.

## Files

- `system_prompt.txt` — complete system prompt used for the agent.
- `test_cases.md` — test scenarios, expected behavior, and evidence status.

## Important note

This is a preliminary qualification demonstration, not a loan approval system. Final eligibility, interest rates, and loan terms must be confirmed by an authorized human loan expert.
