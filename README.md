# Home Credit LAP Voice Agent

## Project Overview

This project implements an AI-powered voice agent using Retell AI for initial Loan Against Property (LAP) eligibility screening.

The agent conducts a natural conversation with customers, collects relevant eligibility information, identifies disqualifying conditions, and routes eligible customers to a loan specialist.

## Objectives

* Conduct a natural and professional customer conversation.
* Verify customer identity before proceeding.
* Assess eligibility using the seven required checks.
* Explain ineligibility politely and end the conversation appropriately.
* Handle busy customers and callback requests.
* Route existing-property-loan or loan-transfer queries to the appropriate specialist.
* Avoid inventing interest rates or guaranteeing loan approval.

## Technology Used

* Retell AI — voice agent creation and testing.
* Large Language Model — conversational reasoning and instruction following.
* System prompting — conversation flow, eligibility rules, and response behavior.

## Eligibility Checks

1. Property type: residential, commercial, or industrial; agricultural property is ineligible.
2. Ownership: sole or joint ownership.
3. Original property documents must be available.
4. Loan amount must not exceed ₹75 lakh, subject to the customer's response when offered the maximum.
5. Salaried or self-employed occupation is accepted; income must be received through a bank account.
6. Estimated current market value of the property is collected.
7. Requested tenure must be between 3 and 15 years, inclusive.

## Conversation Handling

The agent supports callback requests, answers provided out of order, polite disqualification, and referral to a loan-transfer specialist where appropriate.

Eligible customers are referred to a senior loan expert for further discussion. Final approval and exact interest rates are not guaranteed by the agent.

## Testing

The agent was tested against scenarios covering normal eligibility, disqualification conditions, loan amount limits, tenure boundaries, callback handling, existing loans, and out-of-order responses.

See `test-cases.md` for the test scenarios and observed outcomes.

## Demo

Retell AI Voice Orb: https://agent.retellai.com/orb/agent_f47ecd19d267200c7c91876371?token=5b71802de56b97804d137b01798c254e

## Project Files

* `system-prompt.txt` — final agent instructions.
* `test-cases.md` — test scenarios and results.
* `architecture.md` — conversation workflow and decision logic.

## Disclaimer

This is an assignment prototype for initial eligibility screening. It does not represent a formal loan offer, credit decision, or approval from Home Credit.
