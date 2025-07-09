# 📘 Reach the Sky – Business Analyst Case Study

**Role:** Senior Business Analyst  
**Company:** Sky Lending LLC (Partner: Infinity Finance LLC)  
**Industry:** Fintech – Debt Consolidation & Lending  
**Scope:** Design of an end-to-end digital loan application funnel  
**Key Deliverables:** Epics, BDD User Stories, API Specs, Data Flow Diagram, Sprint Structure  

---

## 🧭 Project Overview

Sky Lending launched the *InProgram Loan (IPL)* to help users consolidate debts faster after participating in Infinity Finance’s Debt Resolution Program. After 6+ months in the program, eligible borrowers receive an invitation to complete the IPL application digitally.

The new loan application funnel integrates with multiple external systems and must be flexible to be resumed by representatives via phone (DataCapture360). Once approved, the loan goes directly to the user’s debt account, accelerating the resolution from 3–4 years down to 2–3 months.

---

## 🧱 Functional Structure

I organized the backlog using the following **5 Epics**:

### 🔹 Invitation
- Validation of invitation codes and SSN (last 4 digits)
- Preloading user data from Infinity Finance
- Handling expired or invalid invitations

### 🔹 Generate Offer (PI1 + PI2)
- PI1: Personal Info (name, email, phone, password, T&Cs)
- PI2: Additional Info (DOB, SSN, housing, income, employment)
- E-Sign, Privacy Policy, and Consent handling

### 🔹 Loan Offers
- Integration with **SDG Loan Decisioning Engine**
- Displaying up to 2 loan options (APR, term, origination fee)
- Offer selection and initiation of digital signing (Adobe Sign)

### 🔹 Representatives
- Integration with **DataCapture360** to resume dropped applications
- Full phone-based application flow supported by representatives

### 🔹 Endpoints
- API interactions grouped by system:
  - Infinity Finance
  - SDG Loan Engine
  - DataCapture360
  - Adobe Sign

---

## ✅ Sample BDD User Stories

### 🟦 US-INV-01 – Invitation Validation
Given the user received a valid invitation
And enters the correct SSN last 4 digits
When they submit the form
Then the system validates and redirects to PI1

### 🟩 US-PI2-01 – Additional Info Submission
Given the system retrieved loan options
When the user selects one
Then the system initiates signing via Adobe Sign

### 🟥 US-REP-01 – Resume Application via Phone
Given the user abandoned the flow
And the record exists in DataCapture360
When a representative calls
Then they can resume from the last saved page

---

## 🔗 API Endpoints (Sample Specs)

### 🔹 Infinity Finance
**`POST /api/invitation/validate`**

{
  "invitationCode": "ABC123456",
  "ssnLast4": "1234"
}

### 🔹 SDG Loan Engine
**`POST /api/loan/evaluate`**
{
  "userId": "uuid-user",
  "personalInfo": {
    "dob": "1989-05-10",
    "ssn": "123456789",
    "housingStatus": "rent",
    "income": 54000
  }
}

### 🔹 DataCapture360
GET /api/application/resume?userId=abc123

### 🔹 Adobe Sign
**`POST /api/esign/initiate`**
{
  "userId": "uuid-user",
  "loanOfferId": "offer-001"
}

---

## 🔄 Application Flow Diagram
See Reach the Sky Diagram.pdf (attached) for full flow including:

- Entry point (invitation link)
- PI1 and PI2 forms
- Validation checkpoints
- System interactions
- Inactivity and recovery via phone
- Offer selection and signing

---

## 📦 Sprint Planning
The backlog was divided into 5 sprints, including one focused solely on PI2 and another on representatives’ support.
Dependencies and blockers were clearly marked in Jira using labels and links.
Use cases and API definitions were structured as "dependency" tickets to ensure sequencing and readiness.

---

## ✅ Impact
This structure enabled the engineering team to start development with confidence and clarity:

- Clear story mapping and system boundaries
- Validations, edge cases, and consents documented
- Business logic decoupled from technical constraints
- Visibility across QA, legal, and design

---

## 📬 Contact
Want to learn more or request a portfolio walkthrough?
Feel free to connect on [LinkedIn](https://www.linkedin.com/in/slyleonardo/) or reach out!
