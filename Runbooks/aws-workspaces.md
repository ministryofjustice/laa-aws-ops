#  AWS Workspaces runbook

- **Last review date**: 3nd May 2019
- **Description**: AWS Workspaces are Virtual Desktop Environments for LAA Business Users, Technical Support teams (currently Capgemini), Developers, and a backup for CCMS users. Workspaces replaced Citrix in May 2019 as part of the migration from ATOS to AWS infrastructure.
The primary use for Workspaces is to provide users with access to CIS, Business Objects, TOAD and CFIL [See Register of Technology](https://tech-register.netlify.com) for more details.
AWS Workspaces also currently provide an on-demand method to access CCMS in case of a DOM1 network outage. This is being migrated to instead use the AWS AppStream service, for cost optimisation reasons.
- **Service URL**: [https://clients.amazonworkspaces.com](https://clients.amazonworkspaces.com/)
- **Incident response hours**  9am-6pm on working week days. Weekend support is not currently available.
- **Incident contact details**: Support requests should be raised in our slack channel:  [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD) or directly via [Jira](https://dsdmoj.atlassian.net/secure/CreateIssueDetails!init.jspa?pid=14698&issuetype=3&components=laa-aws-support&priority=3).

- **Service team contact**: Slack: [#laa-ops](https://mojdt.slack.com/messages/CEL68S0LD)
- **Hosting environment**: AWS
- **Out of Hours Support:** There is currently no technical support offered outside business hours. However, in exceptional circumstances, weekend work is possible, following escalation to senior MoJ Digital stakeholders.
- **Restrictions on Access**: This service is currently restricted to LAA Caseworkers and Developers as well as the Capgemini support team. Workspaces are provisioned on an individual per-user basis.
- **Expected speed and frequency of releases**: Workspaces are currently automatically updated with Security patches on at least a monthly basis, although it is not anticipated that these particular updates should have user-visible effects. Once released, routine updates and enhancements to the service will be implemented through our standard Agile Sprint-cycle. If there is an urgent change (such as in the case of a major outage), this will be addressed and further information released as our support team manages the situation.
- **Impact of an outage**: In the event of an AWS Workspaces outage, users would be unable to access CIS, Business Objects, TOAD or CFIL [See Register of Technology](https://tech-register.netlify.com) (currently in Beta). For CCMS **only**, if  DOM1 access is unavailable _and_ AWS Workspaces are not accessible, users will not be able to access this service.

## Contacts

- CIS application: anne-marie.moran@justice.gov.uk

## Useful Links
- [Getting started with Workspaces](https://dsdmoj.atlassian.net/wiki/spaces/aws/pages/1468629070/Getting+started+with+your+AWS+WorkSpaces)
- [Background](https://dsdmoj.atlassian.net/wiki/spaces/aws/pages/1465974863/Workspaces+-+Citrix+Replacement)
- [Process for requesting a workspace](https://dsdmoj.atlassian.net/wiki/spaces/aws/pages/1414922344/Process+for+Requesting+a+new+workspace+new+role)
- [Managing Workspaces for Business Users](https://dsdmoj.atlassian.net/wiki/spaces/LM/pages/1443365352/Managing+Workspaces+for+Business+Users)
- [Workspaces code repository (Private)](https://github.com/ministryofjustice/laa-aws-infrastructure)
- [Register of Technology](https://tech-register.netlify.com) (Currrently in Beta)

