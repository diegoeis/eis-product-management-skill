---
name:
  - Name
version:
  - X.Y.Z
created:
  - YYYY-MM-DD
updated:
  - YYYY-MM-DD
link_jira:
  - $TASK_MANAGER referential URL
---


# {PRD Name}

## TL:DR;

- **What** to solve: 
  - [Describe in at least 2 bullet points what problem we want to solve? What is motivating/stimulating us to create a solution? What pains has the user been feeling?]
- **Why** solve it: 
  - [Describe in at least 2 bullet points the reasons why we want to solve or explore; bullets. Write a maximum of 3 bullet points. If the user sends information, use it.]
- **How** to solve: 
  - [Describe in at least 2 bullet points the descriptions of the solution or hypotheses we will build. If the user hasn't made it clear, ask.]

## Context

[Detailed description of the context divided into 3-4 paragraphs that together should have a maximum total of 250 words, answering: What problem will we solve or opportunity will we explore? What is happening today? What pain exists? Why is this important to the user and what are the beneficial impacts for the business? You can expand and use information from TL:DR, but always ask the user if there isn't enough information. Search the web for similar cases to create a more correct and complete answer.]

### Problem Statements
[Use the format below to list the problems we want to solve. Use user information to suggest common problems this solution will solve. Focus on the problems the user faces. Suggest from web research for real cases and also use information already made in the project itself.]

```
- Customers cannot make their payments effectively
- We still have manual processes in highly sensitive flows
- User has no immediate feedback on completion or payment error via platform
```


## Solution
[2-3 paragraph overview answering: What are we building? Why? For whom? Expected impact? You can expand TL:DR information]

[Describe what the solution is and why it's the best solution. What is the opportunity cost of not doing this? The description of our solution and how it will help the user solve the problem and the company explore this opportunity.]

### Key Features

```
#### Support multiple payment methods
- Cryptocurrency payment: allows users to pay using cryptocurrencies like Bitcoin, ETH and others
- Credit card integration via gateways: to facilitate integration and payment made with card on the platform, without the need to have official regulations.
- Support with digital wallets like Apple Pay and Google Pay: facilitating user adoption without the need to register new information on the platform.
- Payment via PIX: facilitating adoption with payments using copy/paste code and QR Code; 

#### Fraud prevention
- Fraud detection via machine learning: maximally automating the detection of possible fraudulent purchases and preventing money laundering.
- Real-time risk assessment: with fallback to the operations desk when automatic validation fails.

#### Payment via platform
- Payment using balance: customers top up balance on the platform to make payments directly on the platform
- Payment scheduling: user can schedule payments via platform to be executed automatically on a specific day
- Open URL for a third party to pay: customer can share the payment page with the amounts to be paid for other people to make the payment.
```

## General Criteria
[Follow the pattern below. Remember that criteria in a PRD should be high-level descriptions, of operating rules and emphasizing business rules. Define what and not how.]

```
### CRT-1: [scenario name]
- User can filter search results by price range
- Must have possibility to login via social networks
- The system must process and display location updates with maximum latency of 30 seconds for 95% of requests, even with 1000+ simultaneous vehicles
- All sensitive data must be encrypted at rest and in transit, following LGPD and GDPR compliance
- All functionalities must undergo automated security review and manual validation of the 10 most frequent OWASP vulnerabilities.

### CRT-2: [scenario name]

- Uploaded files must allow MP3, WAV and MPG4 formats, with maximum size of 100MB
- The user can listen to the uploaded audio before confirming submission, and corrupted or non-standard files should generate alert and prevent submission
- All sensitive data must be encrypted at rest and in transit, following LGPD and GDPR compliance.
- The product must be bidirectionally integrated with approved external systems, passing integration test scenarios.

### CRT-3: [scenario name]

- Search field should suggest results in real-time with typing error tolerance
- Search results should be presented within 1 second and displayed in paginated pages.
- History of actions performed by the user should be recorded and available upon query in the administrative panel.

### CRT-4: [scenario name]
- User should be able to reset password with email validation in less than 5 minutes
- System should block the account after five failed login attempts and record the event for later query.
```


## Success Indicators
[Suggest and ask the user which indicators should be monitored to understand success.]

```
- Increase payment success by 21%
- Reduce fraud losses by 25%
- Improve customer satisfaction by 30%
- Maintain platform uptime at 99%
```


## Scope

### In Scope
✅ [Item 1]  
✅ [Item 2]  
✅ [Item 3]

### Out of Scope
❌ [Item 1]  
❌ [Item 2]  
❌ [Item 3]

### Future Evolutions
🔮 [Item 1]  
🔮 [Item 2]

## Artifacts and Documentation
- [Link file 1]
- [Link file 2]

## Competitors

[Description of solutions already used in the market by users. Create sections with each competitor, describing their main features and contexts. Follow the pattern below:]

```
### Competitor Name 1

[Competitor Name 1](Website URL)

- Brief description (segment, location, founding date)
- Company size: number of employees, geographic presence, estimated revenue (if public)
- Relevant history and differentiators

#### Main Features
- List of main functionalities or products offered
- Essential characteristics (price, usability, benefits, technical differentiators)
- Support and customer service structure (if applicable)

#### Economics / User Base

- Annual revenue, profit margin or relevant financial data (if public)
- Number of active users/customers (if available)
- Relative market share
- Recent growth or new customer acquisition rate, if possible

```

## Constraints, Assumptions and Risks
[Ask the user if there are any business, technical or product constraints that could make construction difficult or that need to be discussed with areas or stakeholders.]

[Write here the main assumptions and hypotheses about this project. Use information provided by the user, otherwise, ask them at this stage.]

### Business Constraints
[Bullet points with business constraints mapped and provided by the user. If you don't have this information, ask the user.]

### Technical Constraints
[Bullet points with technical constraints mapped and provided by the user. If you don't have this information, ask the user.]

### Risks and Mitigations
[Sections with the topic title and its expanded details about the risks that may exist about this initiative and how they are mitigated.]

---
