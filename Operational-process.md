# --DRAFT--

This is draft document, outlining the AWS Ops team's processes, and based on MoJ Cloud Platform's methodology. This process is continually reviewed and improved.
Please provide all feedback via the LAA Aws ops team's slack channel, or #laa-ops slack channel

## LAA AWS Ops team operational processes

This is a record of the operational processes that we will use to support our users.

## Hours of support

Our hours of providing support are 8am to 6pm, Monday to Friday . During this time we will work on support requests from teams and make sure someone is available to answer questions in [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD)

Outside of these hours we will respond to high priority incidents as per our on call process.

## Working hours

A member of the support team will be available online from 8am to 6pm. This team member may be working remotely, and should be ready to respond to any high priority incidents.

## How does the support sub team work

The support sub team will consist of 2 or 3 engineers. On average each team member will be on the sub team for 2 weeks every 6 weeks.

The key activities for the day are:

#### On starting the day (**TK**) At least one engineer to:

- [ ] Check the #laa-ops  slack channels for any issues to investigate
- [ ] Check the board for any user requests that have been raised and not assigned
- [ ] Get a handover from the on call engineer about any issues out of hours
- [ ] Read through  #laa-aws-webops-team slack channel

#### During support hours (**TK**) At least one engineer to:

- [ ] Actively participate in #laa-ops to field support requests, triage, prioritise and fix

- [ ] *Monitor user support requests being added to the board and triage them for priority*

#### The whole support team to:

- [ ] Manage incident process for incidents in progress

- [ ] Work on user requests for larger work

- [ ] Work on support backlog stories

  #### Before ending the day, at least one engineer to:

- [ ] Handover information about any planned work or in progress high priority incidents to on call engineer

### #laa-ops  Channel

The slack channel is our main entry point for support. We encourage people to ask questions and report problems in this channel and we'll do the best we can to help them.

One engineer should be available to answer questions throughout the hours of support (8AM - 6PM). This will take a bit of co-ordination for lunch etc so the support team should make sure someone is nominated for each period.

#### Communication style

In our responses we should aim to be:

- friendly
- timely

no question is stupid

When the solution is a quick one, it is good to have the whole conversation in the channel rather than in a direct message so that other people can search/see what the resolution was (it might help them or you in the future).

## What we communicate

The main purpose of channel is to discuss the problems that people are having and help them to solve them.

Sometimes it is useful to make broadcast communications, examples include:

- when there is planned work on a service 
- when there is an incident in progress

## In these situations:

Try not to use notifiers like @here and @channel unless absolutely necessary.
Perhaps use visual clues in your message to show it is an announcement
Commit to a time when you will update on the situation and keep that commitment
So for example:

> **ANNOUNCEMENT:**
> As agreed with the relevant teams, the cloud platform team will be upgrading Postgres from version 9.2 (out of support) to version 9.6 on CLA, Moving People Safely and Prison Visits Booking RDS instances today.
>
> We will be doing this work between 10AM and 3PM, we will update at 1PM and 3PM to say how it is going.



## User support tickets

If someone is asking for help that will be quick to do (less than 15 mins) or is mainly advice then keep the interaction in channel and get it done.

If someone needs something that takes longer, is more challenging to complete or you find you've spent longer than 15 mins on it, then continue to talk in the channel but also ask the person asking for help to raise a ticket using the GitHub issue link:



The purpose of the ticket is to keep a record of the work we are doing and how it is progressing. It is not the primary communication channel with the person who raised the problem &emdash; this should remain slack where you can provide a richer and more human interaction, answering questions if necessary. The engineer working on the ticket should update the ticket for our record as work progresses.

In many cases it can be more helpful for the engineer on support to create the ticket rather than the person reporting the problem as you will be able to provide more relevant context.

Once they have created the ticket it will appear in the Support To Do column of our sprint board. It can then be moved into the relevant columns as you work on it.

## What is our incident process

An incident starts when a member of the support team says that it has. It is usually triggered by an alert that indicates a problem. The team member that calls it will send a message saying that there is an incident in progress to #laa-ops.

Support team chooses an incident lead. This person will be the main investigator of the incident. They start to work on the problem, calling on other team members (from the whole team) to help as required.

The rest of the support team communicates the incident out to those who are impacting, including giving updates at regular schedules. The people that they communicate to include:

- Users who are affected by the problem  via #laa-ops
- People in the team who manage communication with senior leadership in MoJ - Nisha, Paddy and Simon Pledger 

In a high priority incident (see below), the support team will gather every 1 hour to work out if additional people/skills are needed and update any external comms.

Once the incident is resolved, the support team will communicate that out and prepare for a post mortem.

#### How do we prioritise incidents?

An incident is a system failure or degradation that has an impact on users.

The size of that impact determines the priority of the incident. At the moment, we find it useful to categories incidents as high priority &emdash; we will begin work on any incident as soon as a member of the support team is available but high priority incidents require greater focus and communication.

## High priority

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

The AWS ops team currently has no on-call process, but we have trialled weekend pagerduty during a major incident. Discussion is ongoing about the possibility of formally implementing weekend on-call duty.

~~Team members who are on call manage an on call rota in pagerduty. Anyone in the team is free to put themselves on the rota.~~

~~The hours of on call are from 5PM - 10AM, with 5PM - 6PM and 9AM - 10AM being additionally covered by a team member from support who is online during those periods.~~

~~On call team members will respond to high priority incidents out of hours and will work on those incidents for up to 1 hour. If the engineer is not able to resolve the issue within that timeframe they will put the service into maintenance mode and put together a plan to resolve the issue in hours.~~

## Where does our documentation live

Our documentation lives in Confluence. This documentation includes architecture, runbooks and common issues.

We are also documenting development into Git repos stored on Github.

## How do we measure how we are doing

### We would like to measure:

* System availability
* Number of incidents and high priority incidents
* Mean time to recovery
* User happiness with support

## Next steps

This document is a work in progress, and we are currently reviewing the following:

- [ ] Review on-call options
- [ ] Review documentation process
- [ ] Review incident management process

