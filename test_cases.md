# Test Cases and Results

Project: Home Credit LAP Voice Agent  
Platform: Retell AI  
Published agent version: V0

**Evidence policy:** Mark a case Pass only after reviewing its transcript or recording. A planned test or an expected outcome is not proof of a pass.

## Test summary

| ID | Scenario | Expected behavior | Evidence/status |
|---|---|---|---|
| TC-01 | Cash income | Explain the offer criteria are not met and end the call promptly. | Recording shared with project owner; review transcript to confirm final behavior. |
| TC-02 | Agricultural property | Disqualify immediately and end the call; do not continue the checklist. | Recording uploaded by project owner; review transcript to confirm. |
| TC-03 | Original documents unavailable | Explain originals are required and end the call; do not continue the checklist. | Recording uploaded by project owner; review transcript to confirm. |
| TC-04 | Customer is busy | Ask for a preferred callback time, acknowledge it, and do not begin eligibility questions. Do not claim a callback was scheduled unless it actually was. | Recording uploaded by project owner; review transcript to confirm. |
| TC-05 | Eligible customer | Gather all seven points, then say a senior loan expert will follow up about exact rates. | Run/retain a complete eligible-customer test and attach evidence. |
| TC-06 | Requested amount exceeds ₹75 lakh | Explain the ₹75 lakh maximum and ask whether the customer wants to proceed with that cap. Continue only if they agree. | Test if not already covered in a retained transcript. |
| TC-07 | Existing property loan / reduce EMI | Tell the customer a loan-transfer specialist will contact them and end the call; do not continue fresh-loan qualification. | Test if not already covered in a retained transcript. |
| TC-08 | Out-of-order answer | Remember information already provided, avoid asking that question again, and return to the earliest unanswered checklist item. | Test if not already covered in a retained transcript. |
| TC-09 | Tenure outside 3–15 years | Explain that the requested tenure does not meet criteria and end the call. | Test if not already covered in a retained transcript. |
| TC-10 | Full conversation and handoff gate | Do not hand off until all seven points are answered and criteria are met. | Confirm from the eligible-customer transcript. |

## Detailed test procedure

### TC-01 — Cash income

**Customer input:** The customer explains that income is received in cash.  
**Expected:** Agent politely explains that the customer does not meet the criteria for this offer and ends the call immediately.  
**Review check:** Ensure there are no further agent responses after the closing statement.

### TC-02 — Agricultural property

**Customer input:** “The property is agricultural land.”  
**Expected:** Immediate disqualification, polite explanation, and call termination. No remaining checklist questions.

### TC-03 — Original documents unavailable

**Customer input:** “I don't have the original property documents available.”  
**Expected:** Immediate disqualification, polite explanation, and call termination. No remaining checklist questions.

### TC-04 — Customer busy

**Customer input:** “I'm busy right now. Could you call tomorrow around 11 AM?”  
**Expected:** Agent asks for/acknowledges a preferred callback time and closes politely without continuing eligibility questions. It must not claim the callback was scheduled unless an actual scheduling action occurred.

### TC-05 — Eligible customer

Use a residential property, sole or joint ownership, originals available, loan amount ₹50 lakh, salaried or self-employed occupation with bank-received income, an estimated market value, and a tenure of 10 years.  
**Expected:** Agent gathers all seven points and states that a senior loan expert will follow up. Do not imply guaranteed approval or invent interest rates.

## Assignment criteria checklist

- [ ] Correct-customer verification and busy/callback handling
- [ ] Present loyalty offer up to ₹75 lakh
- [ ] Ask and remember all seven eligibility items
- [ ] Handle out-of-order answers without asking again
- [ ] Agricultural property disqualification
- [ ] Original-document unavailability disqualification
- [ ] Cash-income disqualification
- [ ] Loan amount cap and customer's choice
- [ ] Tenure 3–15 years inclusive
- [ ] Existing loan / EMI reduction transfer path
- [ ] Natural responses to full sentences, interruptions, and diversions
- [ ] Handoff only after all seven points are answered and eligibility criteria pass
- [ ] Publicly accessible recording and transcript links

## Evidence links

- Google Drive recordings folder: https://drive.google.com/drive/folders/1gSOJqe_zG6RfBOxKqCLo7qzTQW6mXen7?usp=sharing
- Retell AI agent: add a shareable agent link here if available.
- Public individual recording/transcript links: add verified links here after checking access.

## Notes

Update each test row with the actual observed result after reviewing the corresponding transcript. Do not report a test as passed solely because a recording exists.
