**Fund Transfer Feature – Banking App**

**1. Introduction**
This document defines the user stories and acceptance criteria for the Fund Transfer feature in a banking application. The objective is to enable customers to transfer money easily and securely.
The acceptance criteria are defined using both:
•	Simple method
•	BDD (Behavior Driven Development) method
The user stories are also validated using the INVEST principle.
________________________________________
**2. User Story 1 – Add Beneficiary**

As a bank customer, I want to add a beneficiary so that I can transfer money to that account.
________________________________________
**Acceptance Criteria – Simple Method**

•	Customer should be able to enter beneficiary name

•	Customer should be able to enter account number

•	Customer should be able to enter IFSC code

•	System should validate account number

•	System should save beneficiary successfully

•	System should display confirmation message
________________________________________
**Acceptance Criteria – BDD Method**

Scenario: Add beneficiary successfully

Given the customer is logged into the banking app 

When the customer enters valid beneficiary details 

And clicks on Add Beneficiary  

Then the system should save the beneficiary  

And show success message
________________________________________
**3. User Story 2 – Transfer Money**

As a bank customer, I want to transfer money to a beneficiary so that I can send funds easily.
________________________________________
**Acceptance Criteria – Simple Method**

•	Customer should be able to select beneficiary

•	Customer should be able to enter transfer amount

•	System should validate account balance

•	System should complete transfer successfully

•	System should show confirmation message

•	System should update account balance
________________________________________
**Acceptance Criteria – BDD Method**

Scenario: Successful money transfer

Given the customer is logged in  

And customer has sufficient balance 

When customer selects beneficiary

And enters transfer amount  

And clicks Transfer  

Then the system should transfer money  

And show confirmation message  

And update account balance
________________________________________
**4. User Story 3 – View Transaction Confirmation**

As a bank customer, I want to view transaction confirmation so that I can verify successful transfer.
________________________________________
**Acceptance Criteria – Simple Method**

•	System should display transaction ID

•	System should display beneficiary name

•	System should display transfer amount

•	System should display date and time
________________________________________
**Acceptance Criteria – BDD Method**

Scenario: View transaction confirmation

Given the transaction is successful 

When the transfer is completed  

Then the system should display transaction ID  

And beneficiary name  

And amount  

And date and time
________________________________________
**5. INVEST Analysis**

User Story: Transfer Money
________________________________________
Independent
The story can be developed independently without depending on other unrelated features.
________________________________________
Negotiable
Details like transfer limit, OTP validation, and daily limit can be discussed with stakeholders.
________________________________________
Valuable
This feature provides core value to customers by enabling money transfer.
________________________________________
Estimable
The development team can estimate effort based on UI, backend logic, and validation requirements.
________________________________________
Small
The story is small enough to be completed within a sprint.
________________________________________
Testable
The story can be tested with scenarios such as:

•	Successful transfer

•	Insufficient balance

•	Invalid beneficiary
________________________________________
**6. Conclusion**

This document defines the user stories and acceptance criteria for the Fund Transfer feature in a banking application.

Both Simple and BDD methods are used to ensure clarity and testability of requirements. The INVEST principle ensures that the user stories are well-structured, valuable, and ready for development.

This documentation helps ensure effective communication between stakeholders, Business Analysts, developers, and testers, enabling successful delivery of the feature in an Agile environment.

