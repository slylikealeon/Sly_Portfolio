<h1> Reach the Sky Challenge </h1>

<h2> Project Description </h2>
Sky Lending LLC is a partner company of Infinity Finance LLC, an online fintech lending company that helps borrowers access fast, easy, and low-cost credit lines to pay for debts under a program
called Debt Resolution Program. This program consists of a borrower that deposits a monthly sum into an FDIC-insured Dedicated Account, while Infinity Finance negotiates with creditors to lower the
borrower’s debt amount. Once a creditor agrees to the lower amount, funds are withdrawn from the borrower’s FDIC-insured Dedicated Account.
Sky Lending is launching the InProgram Loan (IPL) and has reached us to be their engineer partner and help them build their application funnel.

The goal of the Sky Lending’s IPL is to help their end-user, a borrower experiencing debt, to consolidate their debts and pay off those faster.

IPL works in conjunction with Infinity Lending’s Debt Resolution Program. The end-user must have first participated in this program for at least 6 months before receiving an invitation to apply for IPL.

Upon receiving the invitation, the borrower must complete the Sky Lending’s application process.
While most applicants should be approved as they’ve already met the criteria of 6-month’s participation in Infinity Finance’s debt resolution program, they are still subject to Sky Lending’s credit
policy and verification strategies. 

If the borrower's application is approved, he will receive a loan from Sky Lending that goes directly toward their Infinity Finance Debt Resolution Program to settle their remaining debts. The borrower
then owes Sky Lending as opposed to owing creditors.

Having these funds from Sky Lending allows for Infinity Finance to negotiate better terms with the lenders and creditors that the borrower owes money to, allowing him to achieve debt resolution in 2
to 3 months, as opposed to 3 to 4 years.

Once the borrower receives the invitation link, he will be able to access the Sky Lending’s funnel landing page that will request information such as an invitation code (this should be pre populated
from the invitation link), SSN last four digits, and Affiliate Sharing agreement to review and accept. Infinity Finance will validate the invitation code, SSN, and provide the borrowers personal information from their records.

Once this code is validated, the borrower will be taken to a form in which he will be able to confirm or edit his Personal Information page (PI1) with fields such as first and last name, address, phone,
email and password. Before submitting the form, the borrower will have to agree to the E-Sign Consent, the Terms of Use and the Privacy Policy.

Once the PI1 form is validated and there are no collisions, the borrower will be taken to the Additional Information Page (PI2) where he will need to fill the following information: DOB, SSN,
housing status, time at residence, education, employment status, pay frequency, and annual income. Before submitting the form the borrower will need to agree the E-Sign Agreement, Credit
Authorization Agreement, Terms of Service, and Privacy Policy. The application should disclose that by agreeing and continuing the borrower’s credit score will not be affected.

Sky Lending has decided to use the SDG Loan Decisioning Engine to evaluate the borrower and retrieve the available loan offers (up to two) that apply to this particular borrower. Offers will vary in
payment terms, interest rate, APR, origination fee. In the Offer Page the user will be able to pick the offer that best meets his needs.

Also SDG will provide the DataCapture 360 product, that will allow representatives to call and resume an application if a borrower drops the funnel before selecting an offer.
Also Infinity Finance will provide Sky Lending with a list of selected borrowers to be called by a representative and complete the whole application over the phone.

<h2> Deliverables Requested </h2>

- Use Cases or Epics to be developed

- Define API’s endpoints request/response payloads

- Data Flow Diagram

- User Stories to Develop the PI1 or PI2 pages


<h2> Important </h2>
<a href="https://leonardosly.atlassian.net/jira/software/projects/RS/boards/8/backlog">Link to the project's backlog in Jira</a>

User: userforjira@gmail.com

Password: userforjira

<h2> Epics </h2>

The epics that I have been created were the following:

- Invitation (tickets related to the invitation link to the program).

- Generate offer (including PI1 and PI2).

- Loan offers.

- Representatives (those tickets related to representatives who call users to help them complete the loan application).

- Endpoints (I divided this epic into 4 parts, depending on who to interact with)

-- (Endpoints) - Infinity Finance (for data validation)

-- (Endpoints) - Adobe Sign (for signing documents)

-- (Endpoints) - SDG Loan Decisioning Engine (to validate the client and get the available loan offers)

-- (Endpoints) - DataCapture 360 (to capture when a client leaves an application)


 You will be able to filter the tickets by epic through the Epic panel that is available in the <a href="https://leonardosly.atlassian.net/jira/software/projects/RS/boards/8/backlog">project's backlog</a>.
 
<h2> API’s endpoints request/response payloads </h2>
In the backlog you will find tickets that are called dependencies (it is a type of ticket that indicates that something needs to be developed or a decision is made in order to carry out a user story) and that will represent the different endpoints that are needed.

There are 2 ways to filter and view these tickets:

- Selecting the epics that were mentioned in the previous point.

- Use the "Label" filter in the backlog.

NOTE: Although there are all the titles of the endpoints that are needed, only the tickets that are within the "Sprint PI2" and "Representatives" were those that I had specified.

<h2> User Stories to Develop the PI1 or PI2 pages </h2>
The backlog is divided into 5 sprints, of which I developed all the tickets mentioned in the "Sprint PI2". Although RS-13 is the central ticket of said sprint and it is the one that must be developed, the rest of the tickets are marked as dependencies and are blockers of the aforementioned story.

<h2> Data Flow Diagram </h2>
You will be able to find this diagram in the files attached to this project. I represented not only user activities but also system actions and the relationship with each of the endpoints.
