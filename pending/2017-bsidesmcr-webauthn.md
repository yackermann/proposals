Proposer: Yuriy Ackermann
Year: 2017
Outcome: Pending
Video: 

BSides Manchester Talk Proposal 
===================

Title: WebAuthn - New authentication, for the new web.
Duration: 30 min
Level: Beginner/Intermediate   
Categories: Security, Authentication, Web

Description
===========
Despite all our attempts to make password authentication easy, we are still having issues with user experience, security and adoption of new authentication solutions. To resolve this issue, FIDO Alliance, under W3C mandate, has proposed new, assertion based, authentication protocol, called WebAuthn, and this is what I am going to talk about. 

Objectives
==========
Everyone knows the challenges we are facing with authentication, such as insecure password storage, weak passwords, phishing etc. I will invite participants to rethink authentication. I will present why WebAuthn is the solution to the current authentication problems. I will provide an insight to how it works, and hopefully, by the end, participants will understand why `WebAuthn` is one honking great idea.

Detailed Abstract
=================
### 1: Reviewing current authentication, and where passwords can leak
I will start by introducing current authentication model. We will look at the history of today's authentication, show what is the best thing we can do today, and why we it's not enough.

### 2: Introducing protocols
I'll introduce `WebAuthn` protocol. Step by step will tour audience over four key levels of the protocol

 - User level
 - Client level(`Credential Management API`)
 - Protocol level(`WebAuthn`)
 - Hardware level(`CTAP2`)

On the user level, we will review what user experience we are aiming at, and what do we see as a user friendly authentication.

On the client level, we will do brief introduction to `Credential Management API`, and how `WebAuthn` incorporates into CredManL1 model.

On the protocol level we will explain why Challenge-Response Cryptographic-Signature based protocol is the best approach towards the authentication. We will step-by-step slice the protocol on the pieces, and review protection mechanisms the protocol incorporates. 

On the Hardware level, we will introduce new `Client-to-Authenticator` API, new low-level, a standardized API for driver-less communication with authenticators for assertion based operations.

On basic level, I will provide audience with an easy recipe to cook their own secure/private authentication protocol.

After presenting protocol, we will look at current `WebAuthn` solutions available, which vendor currently support it, and browser support.

### Part 3: Demo
Possibly do demo. Most likely, hopefully.

### Part 4: Conclusion
In this section we will do recap of what we have learned. We will have a quick talk about security considerations that newcomers have to keep in mind before starting to use `WebAuthn`. Overview existing resources/demos/snippets etc.

Outline
=======
##### Intro (2 minutes):

 - Who am I, what do I do.
 - What we are going to talk today about

##### Current authentication intro (3 minutes):

- What is current authentication looks like?
- How we got here?
- Why it fails?

##### WebAuthn (15 minutes)

 - Introducing FIDO organization and what are we doing]
 - Creditential Management API
 - WebAuthn
 - 5 steps to develop secure authentication protocol
 - Introduction to Client-to-Authenticator protocol

##### DEMO (5 min)
##### Conclusion (3 minutes)

 - Security considerations
 - WebAuthn solutions on the market

##### Q & A (10 minutes)

Additional Notes
================
None

Additional Requirements
=======================
None
