Proposer: Yuriy Ackermann
Year: 2016
Outcome:
Video: 

KiwiPyCon Talk Proposal
===================

Title: Universal Second Factor authentication, or why 2FA today is wubalubadubdub?
Duration: 30 min
Level: Beginner/Intermediate   
Categories: Security, Authentication

Description
===========
Passwords get keylogged, phished, guessed, bruteforced, leaked etc. To face this problem we came up with second-factor authentication(2FA). Today main 2FA solutions are OTP(TOTP, HOTP), RSA keys and SMS. All these solutions lack UX, security and privacy, easy to phish, and mostly not standardized. In this talk we will introduce FIDO U2F protocol, talk about its key strength, overview the protocol, review current protocol support, and for desert do some demo. 

Objectives
============
This talk will show why todays `2FA` solutions fail from security and user experience perspective. Everyone at KiwiPyCon probably already know what `2FA` is. I will invite participants to think about the problems `2FA` has, and solution that `FIDO U2F` provides. By the end, participants will understand why `U2F` is one honking great idea. Participants will also learn about some of the legacy tradeoff's they will have to accept, in order to implement U2F in their system that will hopefully lead to improve in security in the long run.

Detailed Abstract
=================
### 1: Why current 2FA solutions are wubalubadubdub?
I'll start by looking at the problem that `2FA` tries to solve: providing secure authentication for the users. I'll introduce issues with current 2FA solutions, and reasons why they are failing. For example, one of the most popular second factor solutions is SMS. This proven to be fairly weak solution for numerous reasons. One of the main is that it is still phishable. If your user had given away his username and password, what would stop user to give away his SMS code? As addition SMS is major privacy concern, and as recent stories show, fairly easy to spoof. 

So todays 2FA solutions sound nice and great from marketing view point, but in reality we are in a lot of problems, and we need to start doing something about it.

### 2: How do we solve it?
I'll introduce FIDO U2F protocol. Step by step will tour audience over `FIDO U2F` protocol. We will start with over-viewing three levels of `FIDO U2F` protocol.

 - User level
 - Client level(i.e. browser etc)
 - Protocol level

On protocol level we will explain why Challenge-Response Public-key cryptography based protocol is the best approach towards the authentication, rather than one time passwords, and this is because challenge response ensures unique signature on every authentication request, and most importantly, removes need for relying party(i.e. Google/Facebook/Yubico etc) know the secret. But Public-Key Challenge-response 2FA does not exactly solve phishing and privacy issues, and so we will discuss phishing protection, registration unique key-pair, defense against cloning and key attestation and other forms of protection `FIDO U2F` incorporates.

On basic level, I will provide audience with an easy recipe to cook their own secure/private `2FA` solution.

After presenting protocol, we will look at current `FIDO U2F` solutions, vendor support, and browser support.

### Part 3: Demo
In this part I will do multiple demos of usage and implementation of `FIDO U2F`, including python Flask(DEMO is ready), Django plugin(In development) and bonus(Secret).

### Part 4: Conclusion
In this section we will do recap of what we have learned. We will have a quick talk about security considerations that newcomers have to keep in mind before starting to use `FIDO U2F`. Describe existing resources/demos/snippets etc.

Outline
=======
##### Intro (2 minutes):
 - Who am I, what do I do.
 - What we are going to talk today about

##### 2FA overview (5 minutes):
 - What is 2FA?
 - What solutions with have today?
 - Why they are failing? 

##### FIDO U2F (13 minutes)
 - Introducing FIDO organisation and what they do.
 - Into to FIDO U2F protocol.
 - 5 steps to develop secure 2FA protocol
 - Security considerations
 - U2F solutions today

##### DEMOS (5 min)
##### Conclusion (3 minutes)
##### Q & A (10 minutes)



Additional Notes
================
None

Additional Requirements
=======================
None
