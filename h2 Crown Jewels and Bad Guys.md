# h2 Crown Jewels and Bad Guys

## x) Read and summarize

### Summary of Hutchins et al 2011:
### Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains

Intelligence-driven computer network defense is a risk management strategy that addresses the threat component of risk, incorporating analysis of adversaries, their capabilities, objectives, doctrine and limitations. It is a continuous process, leveraging indicators to discover new activity with yet more indicators to leverage.

The fundamental element of intelligence in model is the indicator. Indicators can be subdivided into three types: atomic, computed and behavioral.

With respect to computer network attack (CNA) or computer network espionage (CNE), the definitions for these kill chain phases are as follows:
1. Reconnaissance
2. Weaponization
3. Delivery
4. Exploitation 
5. Installation
6. Command and Control
7. Actions on Objectives

Intelligence-driven computer network defense is a nowadays necessity. Conventional, vulnerability-focused processes are insufficient. The intrusion kill chain provides a structure to analyze intrusions, extract indicators and drive defensive courses of actions.

The kill chain shows an asymmetry between aggressor and defender.

#### My own views:

- network defense is lot more than fighting against odd spam emails
- how important is organizations general awareness, this study has been made in security oriented company
  - how to reach that level in companyes whose general business idea is other than security?

### Summary of Shostack 2014:
### Threat Modeling: Designing for Security
### Chapter 1 - Dive in and Threat model!

Threat modeling is about using models to find security problems. Using a model means abstracting away a lot of details to provide a look at a bigger picture, rather than the code itself.

Four key questions:
1. What are you building?
2. What can go wrong?
3. What should you do about those things that can go wrong?
4. Did you do a decent job of analysis?

Building a diagram, finding threats, addressing them, and then checking work. After having a diagram, then looking for what can go wrong with its security. 

STRIDE Mnemonic to Find Threats. It stands for:

**Spoofing** is pretending to be something or someone you're not.
  
**Tampering** is modifying something you're not supposed to modify.
  
**Repudia tion** means claiming you didn't do something.
  
**Denial of Service** are attacks designed to prevent a system from providing service.
  
**Information Disclosure** is about exposing information to people who are not authorized to see it.
  
**Elevation of Privilege** is when a program or user is technically able to do things that they're not supposed to do.
  
Tips for Identifying Threats: Start with external entities, never ignore a threat because it's not what you're looking for right now and focus on feasible threats.

#### Addressing Each Threat:
Mitigating threats
Eliminating threats
Transferring threats
Accepting the risk

Validation of threat model last part.

Questions to check model:
Is this complete?
Is it accurate?
Does it cover all the security decisions we made?
Can I start the next version with this diagram without any changes?

Update the Diagram if needed.

Threat Modeling:
1. Draw a diagram.
2. Use the EoP game to find threats.
3. Address each threat in some way.
4. Check your work with the checklists at the end of this chapter.
5. Celebrate and share your work.

Validating Threats:
1. Have we written down or filed a bug for each threat?
2. Is there a proposed/planned/implemented way to address each threat?
3. Do we have a test case per threat?
4. Has the software passed the test?

#### My own views:

- threat modelling is long term task
- threat model is never fully finished
- how to engage all needed parties (out of tech personnel too) to make sufficient threat model?

## a) Make-belief boogie-man. Create a treath model for imaginary company

#### To do:
#### 1. Create an imaginary company and create threat model.
#### 2. Business requirements come from business, technical specialist help with tech. Inlude this in your narrative.
#### 3. Your analysis should cover all parts of the four question model (four key questions in Threat modeling manifesto)

### Imaginary company

Housing cooperative with about 100 apartments. In this case focus is data gained from electric locking system. System is based on Iloq keys that combines by air keys, door locks, local server and supplier server. It goes without saying that this kind of data contains privacy element.

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/Diagram.JPG)

Simplified diagram

Four key questions repeated:

1. What are you building? 2. What can go wrong? 3. What should you do about those things that can go wrong? 4. Did you do a decent job of analysis?

Some answers:
1. Threat model that secures residents privacy data
2. e.g. privacy data can be accessed unauthorized
3. e.g. determine right state of access rights
4. Bit by bit


## b) Incident analyses

I picked Marriott International case from site: https://www.csoonline.com/article/534628/the-biggest-data-breaches-of-the-21st-century.html

It happened September 2018 and impacted 500 million users.

What happened: "Marriott learned during the investigation that there had been unauthorized access to the Starwood network since 2014. "Marriott recently discovered that an unauthorized party had copied and encrypted information and took steps towards removing it. On November 19, 2018, Marriott was able to decrypt the information and determined that the contents were from the Starwood guest reservation database," the statement added. The data copied included guests' names, mailing addresses, phone numbers, email addresses, passport numbers, Starwood Preferred Guest account information, dates of birth, gender, arrival and departure information, reservation dates, and communication preferences. For some, the information also included payment card numbers and expiration dates, though these were apparently encrypted."

Analysis: Unauthorized access has been happened for long time, many years. Apparently safety measures has been insufficient.

## c) Starting a lab

First I seached info how to show images at github. I found that from page: https://stackoverflow.com/questions/68777239/how-to-display-an-image-in-readme-file-on-github

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/Downloads.JPG)

I started installation by entering: https://terokarvinen.com/2021/install-debian-on-virtualbox/

Then Linux download at page: https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/ and Virtualbox at page: https://www.virtualbox.org/wiki/Downloads

### Virtualbox

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/VirtualboxInstall1.JPG)

I didnt installed asked networking features cause I wanted to try out first without

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/VirtualboxInstall2.JPG)

I continued by following instructions. I used "TeroKarvinenCom" cause I wast sure it was mandatory for further settings.

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/VirtualboxInstall3.JPG)

And so on

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/VirtualboxInstall4.JPG)

And last table of Virtualbox install

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/Virtualbox1.JPG)

Options

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/Virtualbox2.JPG)

Getting ready for Linux!

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/Virtualbox4.JPG)

Powering up

### Linux

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/Linux1.JPG)

Boot menu

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/Linux2.JPG)

Desktop

![Model](https://github.com/bek817/TrusttoBlockchain/blob/main/Linux3.JPG)

Webpage opens too, so I think Virtualbox networking options should not need to install at least for basic browsing.

Environment 6 years old laptop PC

Processor	Intel Core(TM) i7-7700HQ CPU @ 2.80GHz 2.81 GHz, x64

Installed RAM	24,0 Gt

OS Windows10 64-bit

