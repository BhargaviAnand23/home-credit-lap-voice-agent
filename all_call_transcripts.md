# Call Transcripts

All 13 test call transcripts. Each section shows the scenario, call ID, expected result and actual result, followed by the transcript. The matching audio recordings are in the Google Drive folder linked in the README.

---

```text
Scenario: 01 Happy Path
Call ID: call_59a8df1479de734f912b9d7edda
Audio file: 01_Happy_Path.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: All 7 items asked once; qualifies; senior loan expert handoff at the end
Actual result: Pass (call was ended by the customer hanging up)
Note: speech recognition misheard "residential flat" as "residential fact", "original papers" as "original business", and "one crore" as "one course".

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes.
agent: Thank you, Meera. Is this a good time to talk for a
user: Yeah. Sure.
agent: couple of minutes?
agent: We’re calling because you have a Home Credit Loan Against Property offer of up to seventy-five lakh rupees. May I ask a few quick questions to see if
user: Yeah. Go ahead.
agent: it suits you?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: It's a residential fact.
agent: Alright. Is the property in your name alone, or jointly owned?
user: It's in my name only.
agent: Do you have the original property documents available for verification?
user: Yes. I have the original business at home.
agent: What loan amount are you looking for?
user: Around fifty lakhs.
agent: Are you salaried, or do you run your own business?
user: I'm salaried. I work in an IT company.
agent: And is your income received in your bank account, or in cash?
user: My salary comes into my bank account.
agent: Roughly, what’s the current market value of the property?
user: About one course.
agent: Thanks. Over how many years would you like to
user: Maybe ten years.
agent: repay the loan?
agent: Thank you, Meera, that’s everything I needed, and you meet the basic criteria for this offer. A senior loan expert from Home Credit will call you back shortly to explain the exact interest rate and next steps. Thank you for your time, and have a great
user: Thank
agent: day.
user: you.
agent: You’re welcome, Meera. Have a good day.
```

---

```text
Scenario: 02 Joint Ownership and Self-Employed (bank income) - full qualification
Call ID: call_ab4946e0591428755d70f3ae3cb
Audio file: 02_Joint_Ownership_Self_Employed.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Joint ownership and self-employed with bank income accepted; all 7 items asked; handoff at the end
Actual result: Pass (call was ended by the customer hanging up)
Note: speech recognition misheard "originals" as "options", and "one crore" as "one row" / "one course"; the agent asked for a clearer value before moving on.

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes. I'm Mira.
agent: Thanks. Is this a good time to talk for a
user: Yes. Go ahead.
agent: couple of minutes?
agent: Home Credit has a special Loan Against Property offer for existing customers, up to seventy-five lakh rupees. May I ask a few quick questions to see if
user: Sure. Go ahead.
agent: it suits you?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: It's a residential house.
agent: Is the property in your name alone, or jointly owned?
user: It's jointly owned with my husband.
agent: Do you have the original property documents available for verification?
user: Yes. The options are available.
agent: What loan amount are you looking for?
user: I need forty lakhs.
agent: Are you salaried, or do you run your own business?
user: Self employed.
agent: And is your income mainly received in your bank account, or in cash?
user: My payments come into my bank account.
agent: Roughly, what is the current market value of the property?
user: Over one row.
agent: Could you give me a rough value in lakh or crore rupees?
user: One course.
agent: Over one crore, noted. Over how many years would you like to repay the loan?
user: Twelve years?
agent: Thank you, Meera. You meet the basic criteria for this offer. A senior loan expert from Home Credit will call you back shortly to explain the exact interest rate and next steps. Thank you for your time, and
user: Thank
agent: have a great day.
user: you.
agent: You're welcome. Have a good day.
```

---

```text
Scenario: 03 Agricultural Property
Call ID: call_f766c3532c1e04d3742ecc64c11
Audio file: 03_Agricultural_Property.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Disqualified politely as soon as the property is agricultural; no further questions; call ends
Actual result: Pass (call was ended by the customer hanging up)

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes.
agent: Thanks. Is this a good time to talk for a
user: Yeah. Sure.
agent: couple of minutes?
agent: We’re calling about a Loan Against Property offer from Home Credit of up to seventy-five lakh rupees. May I ask a few quick questions to see if it
user: Sure. Go ahead.
agent: suits you?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: It's an agricultural land.
agent: Thank you for sharing that, Meera. Unfortunately, agricultural land doesn’t meet the criteria for this specific offer. I appreciate your time, and have a good day.
user: Okay. Thank you.
agent: Thank you, Meera. Have a good day.
```

---

```text
Scenario: 04 Cash Income
Call ID: call_691ffa13b21747f133c674b183d
Audio file: 04_Cash_Income.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Disqualified politely when income is received mainly in cash; no further questions; call ends
Actual result: Pass (agent ended the call)
Note: speech recognition heard "thirty lakhs" as "thirty bucks"; the agent asked me to confirm instead of assuming.

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes. Speaking.
agent: Is this a good time to talk for a couple of minutes?
user: Yeah. Sure.
agent: We’re calling about a pre-approved Loan Against Property offer of up to seventy-five lakh rupees. May I ask a few quick questions to see if
user: No. Go ahead.
agent: it suits you?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: It's a residential house.
agent: Is the property in your name alone, or jointly owned?
user: It's in my name only.
agent: Do you have the original property documents available for verification?
user: Yes. The originals are available.
agent: What loan amount are you looking for?
user: Around thirty bucks?
agent: Just to confirm, do you mean around thirty lakh rupees?
user: Yes. Thirty lakhs.
agent: Are you salaried, or do you run your own business?
user: I'm self employed. I own a small shop.
agent: And is your income received in your bank account, or in cash?
user: Mostly, my customers pay me in cash.
agent: I’m sorry, Meera, but since your main income is received in cash, you don’t meet the criteria for this specific offer at this time. Thank you for your time, and have
user: Thank you.
agent: a good day.
agent: You’re welcome. Take care.
```

---

```text
Scenario: 05 No Original Documents
Call ID: call_b2aa0a1ad41d58025c6506770a2
Audio file: 05_No_Original_Documents.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Commercial and joint ownership accepted; disqualified politely when only photocopies are available; call ends
Actual result: Pass (agent ended the call)
Note: speech recognition cut "commercial shop" to "commercial show"; the agent asked a clarifying question instead of assuming.

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes. Speaking.
agent: Thank you, Meera. Is this a good time to talk for
user: Yeah.
agent: a couple of minutes?
agent: We’re calling because you have a pre-approved Loan Against Property offer of up to seventy-five lakh rupees. May I ask a few quick questions to see
user: Sure. Go ahead.
agent: if it suits you?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: It's a commercial show.
agent: Do you mean a commercial showroom?
user: It's a shop.
agent: Okay. Is the shop in your name alone, or jointly owned?
user: It's jointly owned. With my brother.
agent: Do you have the original property documents available for verification?
user: I only have photocopies
agent: I’m sorry, Meera, but original property documents are required for this particular offer, so you don’t meet the criteria at this time. Thank you for your time,
user: Okay.
agent: and have a good day.
```

---

```text
Scenario: 06 Tenure Too Short
Call ID: call_3f7ef392858510c72717f58cc70
Audio file: 06_Tenure_Too_Short.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Disqualified politely when tenure is 2 years (below 3), no handoff, call ends
Actual result: Pass (agent ended the call)
Note: speech recognition heard "one crore" as "one crew"; the agent asked me to confirm instead of assuming.

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes. I am.
agent: Thank you, Meera. Is this a good time to talk for a
user: Yeah. Go ahead.
agent: couple of minutes?
agent: We're calling because you have a pre-approved Loan Against Property offer from Home Credit of up to seventy-five lakh rupees. May I ask a few quick questions to see
user: Sure. Go ahead.
agent: if it suits you?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: It's a residential flat.
agent: Is the flat in your name alone, or jointly owned?
user: It's in my name only.
agent: Do you have the original property documents available for verification?
user: Yeah.
user: are available.
agent: What loan amount are you looking for?
user: Around forty lakhs.
agent: Are you salaried, or do you run your
user: I'm
agent: own business?
user: salaried.
agent: And is your salary received in your bank account, or in
user: Yes.
agent: cash?
user: It comes into my bank account.
agent: Roughly, what would you say is the current market value of the flat?
user: About one crew
agent: Did you mean about one crore rupees?
user: Yes.
agent: Over how many years would you like to repay the loan?
user: Two years.
agent: I’m sorry, Meera, but a two-year tenure doesn’t meet the criteria for this offer. Thank you for your time, and have a good day.
user: Thank you.
agent: You're welcome, Meera. Have a good
agent: day.
```

---

```text
Scenario: 07 Tenure Too Long
Call ID: call_a510133223b4fb3aaa9150a42cb
Audio file: 07_Tenure_Too_Long.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Disqualified politely when tenure is 20 years (above 15), no handoff, call ends
Actual result: Pass (call was ended by the customer hanging up)
Note: speech recognition garbled "one crore" ("on crore") and "twenty years" ("Pantias?"); the agent asked me to restate the repayment period before disqualifying.

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes. I am.
agent: Thank you. Is this a good time to talk for
user: Yeah. Go ahead.
agent: a couple of minutes?
agent: We’re calling because you have a Loan Against Property offer from Home Credit of up to seventy-five lakh rupees. I’d like to ask a few quick questions to see if it suits
user: It's alright.
agent: you, is that alright?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: It's a residential flat.
agent: Is the flat in your name alone, or jointly owned?
user: In my name only.
agent: Do you have the original property documents available for verification?
user: Yes.
user: It's available.
agent: What loan amount are you looking for?
user: Around forty lakhs.
agent: Are you salaried, or do you run your
user: I'm
agent: own business?
user: salaried.
agent: And is your salary received in your bank account, or in cash?
user: It comes into my bank account.
agent: Roughly, what would you say is the current market value of the flat?
user: It's on crore.
agent: Got it. Over how many years would you like to repay the loan?
user: Pantias?
agent: Could you tell me the repayment period in years, for example between three and fifteen years?
user: It's twenty years.
agent: I’m sorry, Meera, a twenty-year tenure doesn’t meet the criteria for this offer, which allows up to fifteen years. Thank you for your time, and have a good day.
user: Thank you.
agent: You’re welcome. Take care.
```

---

```text
Scenario: 08 Loan Above Limit
Call ID: call_18524331e89b926a76d6ada83be
Audio file: 08_Loan_Above_Limit.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Not disqualified at 90 lakh, limit of 75 lakh explained and offered, 15-year tenure accepted, handoff at the end
Actual result: Pass (call was ended by the customer hanging up)
Note: speech recognition misheard "the originals are available" as "All chairs are available"; the customer's "Yes." just before it had already confirmed the documents.

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes. This is.
agent: Thank you, Meera. Is this a good time to talk for a
user: Yeah. Go ahead.
agent: couple of minutes?
agent: We're calling about a pre-approved Loan Against Property offer of up to seventy-five lakh rupees for existing Home Credit customers. May I ask a few quick questions to see if it
user: Sure. Go ahead.
agent: suits you?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: It's residential house.
agent: Is the property in your name alone, or
user: Mine only.
agent: jointly owned?
user: Mine
agent: Do you
user: only.
agent: Do you have the original property documents available for verification?
user: Yes.
user: All chairs are available.
agent: What loan amount are you looking for?
user: I need ninety lakhs.
agent: This offer is available for up to seventy-five lakh rupees. Would you like to proceed with seventy-five lakh rupees?
user: Okay. Seventy five is fine.
agent: Are you salaried, or do you run your own business?
user: Salary.
agent: Is your salary received in your bank account, or in cash?
user: Bank.
agent: Roughly, what is the current market value of the property?
user: About one and a half
agent: About one and a half crore rupees, correct?
user: Yes.
agent: Over how many years would you like to repay the loan?
user: Fifteen years.
agent: Thank you, Meera, that's everything I needed, and you meet the basic criteria for this offer. A senior loan expert from Home Credit will call you back shortly to explain the exact interest rate and next steps. Thank you for your time, and have a great day.
user: Thank you.
agent: You're welcome. Have a great day.
```

---

```text
Scenario: 09 Existing Loan
Call ID: call_ff581f4aff12e0b607716d84dac
Audio file: 09_Existing_Loan.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Transfer specialist message, no further eligibility questions, call ends
Actual result: Pass (call was ended by the customer hanging up)

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yeah.
agent: Thank you, Meera. Is this a good time to talk for a couple of minutes?
user: Yeah. Go ahead.
agent: We’re calling because you have a pre-approved Loan Against Property offer of up to seventy-five lakh rupees. May I ask a few quick questions to see
user: Sure. Go ahead.
agent: if it suits you?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: It's a residential flat.
agent: Is the flat in your name alone, or jointly owned?
user: Actually, I already have it loan running on this property.
agent: Thank you for letting me know. Since there’s already a loan on the property, our loan transfer specialist will contact you shortly to help you with this. Thank you for your time, Meera.
user: Thank you.
agent: You’re welcome, Meera. Have a good day.
```

---

```text
Scenario: 10 EMI Reduction
Call ID: call_40ca12e418e409a7902193649dd
Audio file: 10_EMI_Reduction.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Transfer specialist message, no further eligibility questions, call ends
Actual result: Pass (call was ended by the customer hanging up)
Note: speech recognition misheard "residential" as "Restention" / "restoration"; the agent asked a clarifying question instead of assuming.

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yeah. This is
agent: Thank you. Is this a good time to talk for
user: Yeah. It's good time to
agent: a couple of minutes?
user: talk to you.
agent: We're calling about a pre-approved Loan Against Property offer of up to seventy-five lakh rupees. May I ask a few quick questions to see
user: Yeah. Go ahead.
agent: if it suits you?
agent: What type of property would you be taking the loan
user: Restention.
agent: against: residential, commercial, or industrial?
user: It's a restoration.
agent: Do you mean it’s a residential property, like a house or flat?
user: It's a house, residential house.
agent: Is the property in your name alone, or jointly owned?
user: Actually, I just want to reduce my current EMI.
agent: Since you’d like to reduce your current EMI, our loan-transfer specialist will contact you shortly to help. Thank you for your time, Meera.
user: Thank you.
agent: You're welcome. Have a good day.
```

---

```text
Scenario: 11 Busy Customer
Call ID: call_075724110ea29aa471b68f2a7ec
Audio file: 11_Busy_Customer.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Pitch stopped, callback time asked and confirmed, call ends
Actual result: Pass (callback confirmed; call was ended by the customer hanging up)

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes. This is.
agent: Thank you, Meera. Is this a good time to talk for a couple of minutes?
user: A meeting right now. Can you call later?
agent: Certainly, I understand. What would be a convenient time for us to call you back?
user: Call me in an hour.
agent: All right, we'll call you back in an hour. Thank you, Meera.
user: Thank you.
agent: You're welcome. Have a good evening.
```

---

```text
Scenario: 12 Diversion, Ambiguity and Correction
Call ID: call_f013fe454238e4b9ad00568a8ca
Audio file: 12_Diversion_And_Correction.wav
Agent: Ananya   |   Customer: Meera (played by me)
Expected result: Interest-rate question answered without a number, vague documents answer clarified, corrected tenure (12 years) used, handoff only at the end
Actual result: Pass (call was ended by the customer hanging up)
Note: speech recognition garbled my correction ("ten years... no, make it twelve" appears as "Can you use no. Make it a twelve."); the agent still recorded twelve years.

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: Yes. This is
agent: Thank you, Meera. Is this a good time to talk for a couple of minutes?
user: Yes. Go ahead.
agent: We're calling because you have a Home Credit Loan Against Property offer of up to seventy-five lakh rupees. May I ask a few quick questions to see if it
user: Sure. Go ahead.
agent: suits you?
agent: What type of property would you be taking the loan against: residential, commercial, or industrial?
user: Before that, what's the interest rate?
agent: The exact interest rate will be shared by our senior loan expert after this quick preliminary check. What type of property would you be taking the loan against?
user: Residential house.
agent: Is the property in your name alone, or jointly owned?
user: Mine only.
agent: Do you have the original property documents available for verification?
user: I think the papers are somewhere at home.
agent: Are the original property papers available, or do you only have photocopies?
user: Yes. The originals are available.
agent: What loan amount are you looking for?
user: Forty lakhs?
agent: Are you salaried, or do you run your own business?
user: Yes. Salaried.
agent: And is your income received in your bank account, or in cash?
user: In my bank account.
agent: Roughly, what would you say is the current market value of the property?
user: Eighty lakhs.
agent: Over how many years would you like to repay the loan?
user: Can you use no. Make it a twelve.
agent: Twelve years works. Thank you, Meera, you meet the basic criteria for this offer. A senior loan expert from Home Credit will call you back shortly to explain the exact interest rate and next steps. Thank you for your time, and have a
user: Thank you.
agent: great day.
agent: You're welcome. Have a good day.
```

---

```text
Scenario: 13 Wrong Person
Call ID: call_56b4595c7f852b2be7f1b5e1d0e
Audio file: 13_Wrong_Person.wav
Agent: Ananya   |   Customer: Meera (played by me, as Meera's sister)
Expected result: No loan details shared, callback time asked, call ends
Actual result: Pass (no loan details shared, callback time noted; call was ended by the customer hanging up)

--- Transcript ---
agent: Hello, am I speaking with Meera? This is Ananya calling from Home Credit.
user: No. This is her sister. She's not available.
agent: I’m sorry for the inconvenience. What would be a convenient time for us to call Meera back?
user: Maybe tomorrow evening?
agent: Tomorrow evening works. Thank you, we'll call Meera then. Have a good day.
user: Thank you.
agent: You’re welcome. Have a good day.
```
