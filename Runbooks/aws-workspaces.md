#  AWS workspaces runbook

- **Last review date**: 3nd May 2019
- **Description**: AWS Workspaces are virtual desktop environments for LAA business users and technical support teams (currently Capgemini). Workspaces replaced Citrix in May 2019 as part of the migration from ATOS to AWS infrastructure.
The primary use for Workspaces is to provide users with access to CIS, Business Objects, TOAD and CFIL [See Register of Technology](https://tech-register.netlify.com) form more details.
AWS Workspaces also provide an on-demand method to access CCMS in case of a DOM1 network outage. This uses AWS' Appstream service.
- **Service URL**: [https://clients.amazonworkspaces.com](https://clients.amazonworkspaces.com/)
- **Incident response hours**  9am-6pm on working days. Weekend support is not currently available.
- **Incident contact details**: Support requests should be raised in our slack channel:  laa-aws-support or directly [via Jira](https://dsdmoj.atlassian.net/secure/CreateIssueDetails!init.jspa?pid=14698&issuetype=3&components=laa-aws-support&priority=3) 

- **Service team contact**: Slack: laa-aws-support
- **Hosting environment**: AWS
- **Out of Hours Support:** There is currently no technical support offered outside business hours. However, in exceptional circumstances, weekend work is possible, following escalation to senior MoJ Digital stakeholders.
- **Restrictions on Access**: This service is currently restricted to LAA Caseworkers and developers in our Capgemini support teams. Workspaces are provisioned for each individual user.
- **Expected speed and frequency of releases**: Once released, routine updates and enhancements to the service will be implemented through our fortnightly sprint-cycle. If there is an urgent change (such as in the case of a major outage), this will be addressed and released as soon as our support team becomes available.
- **Impact of an outage**: In the event of an AWS Workspaces outage, users would not be able to access CIS, Business Objects, TOAD or CFIL [See Register of Technology](https://tech-register.netlify.com) (currently in Beta). **CCMS** If  DOM1 access is unavailable _and_ AWS Workspaces go down, users will not be able to access CCMS.

## Useful Links
- [Getting started with Workspaces](https://dsdmoj.atlassian.net/wiki/spaces/aws/pages/1468629070/Getting+started+with+your+AWS+WorkSpaces)
- [Background](https://dsdmoj.atlassian.net/wiki/spaces/aws/pages/1465974863/Workspaces+-+Citrix+Replacement)
- [Process for requesting a workspace](https://dsdmoj.atlassian.net/wiki/spaces/aws/pages/1414922344/Process+for+Requesting+a+new+workspace+new+role)
- [Managing Workspaces for Business Users](https://dsdmoj.atlassian.net/wiki/spaces/LM/pages/1443365352/Managing+Workspaces+for+Business+Users)
- [Workspaces code repository (Private)](https://github.com/ministryofjustice/laa-aws-infrastructure)
- [Register of Technology](https://tech-register.netlify.com) (Currrently in Beta)

