# Home Credit LAP Qualification Voice Agent

Prompt-engineering assignment for SalesAgents AI (AI Intern, Prompt Engineer).
A voice agent ("Ananya") calls an existing Home Credit customer about a pre-approved Loan Against Property offer of up to 75 lakh, runs a 7-point eligibility check, and hands qualified customers to a senior loan expert.

Built and tested on Retell AI (single-prompt agent, web test calls).

## Contents

| File | What it holds |
|---|---|
| `system_prompt.txt` | The full system prompt used for every test call |
| `all_call_transcripts.md` | All 13 test call transcripts, each with scenario, call ID, expected and actual result |
| `Retell_Single-Prompt_Agent_v1.json` | Retell export of the final published version (v1) with an improved call-ending instruction. The test recordings were made with the earlier version (v0), whose prompt is `system_prompt.txt` |

Google Drive folder with the 13 audio recordings, transcripts and screen recording: [Open the Drive folder](https://drive.google.com/drive/folders/1l4ikzu60xQVaba4bQ0sL-aYne-2Vpx-q?usp=drive_link)

## How the prompt works

1. **Identify and check availability.** Confirms the customer, handles busy customers (callback time) and wrong persons (no loan details shared).
2. **Present the offer** in two short sentences.
3. **Turn algorithm on every reply:** extract every fact given, validate it, check for disqualification, check for loan transfer, check the loan limit, update state, then ask only the first missing checklist item.
4. **Seven checklist items:** property type, ownership, original documents, loan amount, occupation and income mode, market value, tenure.
5. **Immediate disqualification:** agricultural property, no original documents, cash income, tenure under 3 or over 15 years.
6. **Transfer branch:** an existing loan or a wish to reduce EMI ends the fresh-loan flow with a loan-transfer specialist message.
7. **Loan limit:** above 75 lakh is not a disqualification; the agent explains the limit and offers the maximum.
8. **Handoff gate:** the senior-expert handoff happens only after all 7 items are answered and every criterion is met.
9. **Guardrails:** no invented rates, fees or minimum property value; product answers come only from the retrieved context; agent gender and language follow the variables.

## Test results

| # | Scenario | Result |
|---|---|---|
| 01 | Happy path | Qualified, handoff |
| 02 | Joint ownership, self-employed, bank income | Qualified, handoff |
| 03 | Agricultural property | Disqualified |
| 04 | Cash income | Disqualified |
| 05 | No original documents | Disqualified |
| 06 | Tenure 2 years | Disqualified |
| 07 | Tenure 20 years | Disqualified |
| 08 | Loan 90 lakh, accepts 75 lakh, tenure 15 years | Limit explained, qualified |
| 09 | Existing loan | Transfer message |
| 10 | EMI reduction | Transfer message |
| 11 | Busy customer | Callback time confirmed |
| 12 | Interest-rate question, vague documents answer, tenure correction | Answered without a rate, clarified, 12 years recorded, handoff |
| 13 | Wrong person | No loan details shared, callback time noted |

## Known limitations

- The agent ended the call herself in 3 of the 13 calls; in the others the call was ended by the tester hanging up. A stronger instruction to call the end-call function immediately after the closing line is the identified fix.
- No recording shows several answers given in one reply and not re-asked; that behaviour is written into the prompt but was not captured on a call.
- Some transcripts contain speech-recognition errors (for example "one crore" heard as "one course"); the agent usually asked for confirmation.
