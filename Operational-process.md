## Operational processes
 
This is a record of the operational processes that we will use to support our users.
 
## User FAQs
 
### How do I request support?
You can get support by posting in [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD) channel or by raising a ticket directly in our AWS or 6dg/RedCentric Jira boards:
- [AWS Ops Jira board](https://dsdmoj.atlassian.net/secure/RapidBoard.jspa?rapidView=262)
- [6DG Ops Jira board](https://dsdmoj.atlassian.net/secure/RapidBoard.jspa?rapidView=265&selectedIssue=LM-3975) - Note: set the _component_ to laa-6dg-support
 
### How long will it take to resolve issue?
Ops team to notify receipt of ticket to requestor/service teams within 2 hrs
Priority will be given to PROD or severity 1/2 issues
Other issues will be addressed in order of priority and availability of resource
If the issue is infrastructure related, a support call will be raised with relevant third party
i.e. AWS, 6dg or RedCentric

### How do I escalate resolution of my issue?
In the first instance request an update on the [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD) Slack channel
Otherwise contact Simon Pledger or Paddy Dewhurst.

## Hours of support
 
LAA Ops team works from 8am to 6pm, Monday to Friday. During this time we will work on support requests from teams and ensure someone is available to answer questions in [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD). The team member who responds may be working remotely.
 
6DG Ops supports the following environments:
- UAT, Pre-Prod/Stage and PROD applications hosted on 6dg infrastructure (CCMS, CIS, MI, CWA, ERIC)
- Dev/Test environments for these applications currently hosted in RedCentric.
 
## How does the support sub team work
 
We assign one engineer and one DBA to support requests in working hours. This support sub-team will triage incident requests raised to them in the [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD) or laa 6dg ops slack channels.
 
The key activities for the day are:
 
#### On starting the day, at least one LAA AWS Ops engineer to:
 
- [ ] Check the #laa-ops slack channels for any issues to investigate
- [ ] Check the board for any user requests that have been raised and not assigned
- [ ] Get a handover from the on-call engineer about any issues out of hours~ if on-call support is being provided
- [ ] Read through [#laa-aws-webops-team](https://mojdt.slack.com/messages/CDTDZ2SN8). I think we should remove this as all should be in laa-ops
- [ ] Review team channels for any reports from engineer covering post-5pm support of previous working Friday -I think we should remove this
 
#### On starting the day, at least one LAA 6dg Ops engineer to:
 
- [ ] Check the #laa-ops slack channels for any issues to investigate
- [ ] Check the LAA 6dg Support Jira board for any user requests that have been raised and not assigned
- [ ] 6dg Ops duty consultant (DC) acknowledges receipt of ticket to service teams within (max) 2 hrs and either
     a) actions ticket if straightforward OR
     b) raises in daily stand-up to assign appropriate 6dg Ops resource
- [ ] Gets a handover from the on-call engineer about any issues out of hours if on-call support is being provided
- [ ] Review team channels for any reports from engineer covering post-5pm support of previous working Friday
- [ ] Carry out standard monitoring
 
#### During support hours at least one engineer to:
 
- [ ] Actively participate in #laa-ops to field support requests, triage, prioritise and fix
- [ ] _Monitor user support requests being added to the board and triage them for priority_
 
#### The whole support team to:
 
- [ ] Manage incident process for incidents in progress
- [ ] Work on user requests for larger work
- [ ] Work on support backlog stories
 
 #### Before ending the day, at least one engineer to:
 
- [ ] Handover information about any planned work or in progress high priority incidents to on-call/post-5pm engineer
 
### #laa-ops channel
 
The slack channel is our main entry point for support. We encourage people to ask questions and report problems in this channel and we'll do the best we can to help them.
 
One engineer should be available to answer questions throughout the hours of support (8am - 6pm). This will take a bit of co-ordination for lunch, etc. so the support team should make sure someone is nominated for each period.
 
When the solution is a quick one, it is good to have the whole conversation in the channel rather than in a direct message so that other people can search/see what the resolution was (it might help them or you in the future).
 
## Triage
 
If a request is likely to take less than 15 mins, or is mainly advice, then keep the interaction within the [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD) channel and get it done.
 
If someone needs something that takes longer, is more challenging to complete or you find you've spent longer than 15 mins on it, then continue to talk in the channel but also raise a ticket in Jira, and then inform the product manager that you will need to begin working on this.
 
The purpose of the Jira ticket is to keep a record of the work we are doing and how it is progressing. It is not the primary communication channel with the person who raised the problem; this should remain slack where you can provide a richer and more human interaction, answering questions if necessary. The engineer working on the ticket should update the ticket for our record as work progresses.
 
In many cases it can be more helpful for the engineer on support to create the ticket rather than the person reporting the problem as you will be able to provide more relevant context.
 
Once they have created the ticket it will appear in the To Do column of our Jira board. It can then be moved into the relevant columns as you work on it.
 
## What is our incident process?
 
An incident starts when a member of the support team says that it has. It is usually triggered by an alert that indicates a problem. The team member that calls it will send a message saying that there is an incident in progress to [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD).
 
Support team chooses an incident lead. This person will be the main investigator of the incident. They start to work on the problem, calling on other team members (from the whole team) to help as required.
 
The rest of the support team communicates the incident out to those who are impacting, including giving updates at regular schedules. The people that they communicate to include:
 
- Users who are affected by the problem  via [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD)
- People in the team who manage communication with senior leadership in MoJ - Nisha, Paddy and Simon Pledger (for STEC/6dg-related issues)
 
In a high priority incident (see below), the support team will gather every hour to work out if additional people/skills are needed and update any external comms.  I don’t think we should add this
 
Once the incident is resolved, the support team will communicate that out and prepare for a post mortem.
 
#### How do we prioritise incidents?
 
An incident is a system failure or degradation that has an impact on users.
 
The size of that impact determines the priority of the incident. At the moment, we find it useful to categories incidents as high priority we will begin work on any incident as soon as a member of the support team is available but high priority incidents require greater focus and communication.
 
#### High priority
 
* Service outages of user facing services
* Slowdown or degradation of service on a user facing service
* Failure of a system that stops one or more teams from working
* Failure of a system that creates a major vulnerability in the cloud platform
 
### How we do postmortems
 
In the AWS Ops team we follow the practice of better understanding system failures through blameless postmortems.
 
The point of a post mortem is to understand the various factors that led up to a system failure and to try to identify things that can be improved to try to stop a similar event occurring in future.
 
Our approach to postmortems is to:
 
* For high priority incidents to hold a group session as soon as possible after the incident is closed
* Develop a timeline of the activities that led to the incident and its resolution
* Walkthrough that timeline and use it to identify opportunities for improvements
* Emerge with a prioritised list of improvements to be made, with owners
* Write up and publish the postmortem, giving a record of the timeline and any actions that have been agreed
 
We currently publish our postmortem reports on Confluence, and will look for a public-facing means to do this.
 
## How we do on call
 
The AWS ops team currently has no on-call process, but we have trialled weekend PagerDuty during a major incident. Discussion is ongoing about the possibility of formally implementing weekend on-call duty.
 
## Where does our documentation live
 
Our documentation lives either in Confluence or here in this repository. This documentation includes architecture, runbooks and common issues.
 
## Performance and Metrics
 
### We currently measure:
*  Time to resolution.
*  Time at each stage; To-Do, In Progress, Done
 
### We would like to measure:
 
* System availability
* Number of incidents and high priority incidents
* User happiness with support
 
## Next steps
 
This document is a work in progress, and we are currently reviewing the following:
 
- [ ] Review documentation process
- [ ] Review incident management process
