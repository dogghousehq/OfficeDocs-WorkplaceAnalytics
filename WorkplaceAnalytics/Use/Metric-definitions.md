---
# Metadata Sample
# required metadata

title: Workplace Analytics metric definitions 
description: Describes the metrics for queries that are available in Workplace Analytics, including Person, Meeting, Group-to-group, and Person-to-group query metrics
author: madehmer
ms.author: v-midehm
ms.date: 08/15/2019
ms.topic: article
localization_priority: normal 
ms.prod: wpa
---

# Metric descriptions for Workplace Analytics

You can use the following metrics in Workplace Analytics to customize your queries.

## Person metrics

|Metric|Description|Query type|Data type|Customizable|
|------|-----------|----------|---------|------------|
|After-hours collaboration|Number of hours the person spent in meetings and on email outside of working hours. **Note**: To target or filter for after-hours collaboration, you can use a filter with the Collaboration hours metric.|Person|Hour|No|
|After-hours email hours|Number of hours the person spent sending email outside of working hours.|Person|Hour|No|
|After-hours meeting hours|Number of hours the person spent in meetings outside of working hours.|Person|Hour|Yes|
|Calls| Total number of calls the person spent time in as initiator or participant, through Teams, during and outside of working hours.| Person| |Count| Yes
|Collaboration hours|Number of hours the person spent in meetings and on email with at least one other person. Collaboration hours include both internal and external hours. |Person|Hour|Yes|
|Collaboration hours external|Number of hours the person spent in meetings and on email with at least one person outside the company (as defined by the participant’s email domains).|Person|Hour|No|
|Conflicting meeting hours|Number of meeting hours where the person had overlapping meetings in their calendar. The count includes the entire duration of all overlapping meetings, not just the amount of time that overlaps. (This number includes all non-declined meeting times, which includes accepted, tentative, or no responses to meeting invitations.)|Person|Hour|Yes|
|Email hours|Number of hours the person spent sending and receiving emails.|Person|Hour|Yes|
|Emails sent|Number of emails the person sent.|Person|Count|Yes|
|External network size|Number of people external to the company with whom the person had at least two meaningful interactions (a meeting or email between five or fewer people) within the last 28 days (or if reported by month, within the last month).|Person|Count|Yes|
|Generated workload email hours|Number of email hours the person created for internal recipients by sending emails.|Person|Hour|Yes|
|Generated workload email recipients|Number of internal recipients on all emails sent by the person. (Counts each recipient once for each email received.)|Person|Count|Yes|
|Generated workload meeting attendees|Number of internal attendees in meetings organized by the person. (Counts each attendee once for each meeting.)|Person|Count|Yes|
|Generated workload meeting hours|Number of meeting hours the person created for internal attendees by organizing meetings.|Person|Hour|Yes|
|Generated workload meetings organized|Number of internal meetings organized by the person.|Person|Count|Yes|
|IMs | Total number of instant messages (IMs) or chats sent by the person as the initiator, through Teams, during and outside of working hours. Note: Time in IM compose estimated to 22 seconds, Time in IM read estimated to 8 seconds| Person| Count| Yes
|Internal network size|Number of people within the company with whom the person had at least two meaningful interactions (a meeting or email between five or fewer people) within the last 28 days (or if reported by month, within the last month).|Person|Count|Yes |
|Low-quality meeting hours|Number of meeting hours in which an attendee multitasked, attended a *conflicting meeting*, or attended a meeting that exhibits *Redundancy (organizational)*. Workplace Analytics admins can [set the hourly rate](settings.md#hourly-rate) of low-quality meeting time; if this value has not been set, the cost defaults to $75 per person hour. |Person|Hour|Yes|
|Manager coaching hours 1:1|Number of hours that a manager spends in one-on-one meetings with their direct reports. |Person|Hour|Yes|
|Meeting hours|Number of hours the person spent in meetings with at least one other person.|Person|Hour|Yes|
|Meeting hours with manager|Number of meeting hours where attendees included at least the person and their manager.|Person|Hour|Yes|
|Meeting hours with manager 1:1|Number of meeting hours involving only the person and their manager.|Person|Hour|Yes|
|Meetings hours with skip level|Number of meeting hours that the person attends where their manager's manager also attends the meeting.|Person|Hour|Yes|
|Meetings|Number of meetings the person attended.|Person|Count|Yes|
|Meetings with manager|Number of meetings where attendees include at least the person and their manager.|Person|Count|Yes|
|Meetings with manager 1:1|Number of meetings involving only the person and their manager.|Person|Count|Yes|
|Meetings with skip level|Number of meetings where the manager of the person's manager is an attendee.|Person|Count|Yes|
|Multitasking meeting hours|Number of meeting hours where the person sent:<ul><li>Two or more emails sent per meeting hour</li><li>Two or more emails sent per meeting for meetings less than one hour</li></ul>|Person|Hour|Yes|
|Networking outside company|Number of companies outside their own that the person had meaningful interactions with, within the last 28 days (or if reported by month, within the last month).|Person|Count|Yes |
|Networking outside organization|Number of departments outside their own that the person had meaningful interactions with, within the last 28 days (or if reported by month, within the last month).|Person|Count|Yes |
|Open 1-hr blocks|Number of one-hour blocks in the person’s calendar without meetings during the work day.|Person|Count|Yes|
|Open 2-hr blocks|Number of two-hour blocks in the person’s calendar without meetings during the work day.|Person|Count|Yes|
|Redundant meeting hours (organizational) |Number of meeting hours a person spent with attendees from three or more distinct levels within that person’s organization. Used in calculating *Low quality meeting hours*.  |Person|Hour|Yes|
|Redundant meeting hours (lower level) |Number of meeting hours a person spent in a meeting with both their manager and their skip-level manager present in the meeting. <br> <br> This metric is _not_ used in calculating *Low-quality meeting hours*. Analysts can use this metric only when creating [Person queries](../tutorials/person-queries.md).|Person | Hour| Yes |
|Time in calls after hours | Number of hours the person spent in calls, through Teams, outside of working hours. For calls that started during working hours, this number only includes the part of the call that occurred outside of that person’s work schedule (as set in Outlook).| Person| Hour| Yes |
|Time in IMs after hours| Number of hours the person spent in reading/sending Instant Messages in  Teams, outside of that person’s working hours. Note: Time in IM compose estimated to 22 seconds, Time in IM read estimated to 8 seconds| Person| Hour| Yes |
|Time in meetings during after hours|Number of hours the person spent in meetings outside of working hours.|Person|Hour|Yes|
|Time in meetings during working hours|Number of hours the person spent in meetings during working hours.|Person |Hour |Yes|
|Time in self-organized meetings|Number of hours spent in meetings organized by the person with at least one other person.|Person|Hour|Yes|
|Total call hours | Total number of hours the person spent in calls as initiator or participant, through Teams, including scheduled and impromptu calls during and outside of working hours (as set in Outlook). | Person| Hour| Yes |
|Total IM hours | Total number of hours the person spent in IMs as initiator or participant, through Teams, including scheduled and impromptu IMs during and outside of working hours (as set in Outlook).  Note: Time in IM compose estimated to 22 seconds, Time in IM read estimated to 8 seconds.| Person| Hour| Yes |
|Total emails sent during meeting | Number of emails the person sent during meetings. |Person|Count|Yes|
|Total focus hours|Total number of hours with two or more hour blocks of time where the person had no meetings.|Person|Hour|Yes|
|Working hours collaboration hours|Number of hours the person spent in meetings and sending emails during working hours.|Person|Hour|No|
|Working hours email hours|Number of hours the person spent in sending email during working hours.|Person|Hour|Yes|
|Working hours in calls| Total number of hours a person spent time in scheduled and unscheduled calls with Teams, during working hours. | Person| Hour| Yes |
|Workweek Span|Time between the person's first sent email or meeting attended and the last email or meeting for each day of the work week. The total number of hours are based on the person’s work week that is set in Outlook, which the user can change at any time. If a work week is not defined in Outlook (or Workplace Analytics is unable to access a user’s Outlook settings), the totals are based on the default of Monday through Friday, with a minimum of four hours and a maximum of 16 hours per day. If reported for the week, the metric is a sum of the daily values for the week. If reported for the month, the metric is the sum of the daily values for the month. |Person|Hour|No|

## Meeting metrics

|Metric|Description|Query type|Data type|Customizable|
|------|-----------|----------|---------|------------|
|Attendee meeting hours|Total number of adjusted meeting hours for all attendees.<br>A _meeting query_ focuses on the meeting as the main entity and reports on the various meeting attributes; a _person query_ looks from a person's perspective and aggregates multiple meetings for the selected time period. Because the two query types have different purposes, their output also differs. |Meeting|Hour|Yes|
|Attendees|Number of people who attended the meeting.|Meeting|Count|Yes|
|Attendees multitasking|Number of attendees that sent emails during the meeting.<ul><li>In meetings of one hour or less, two or more emails.</li><li>In meetings longer than one hour, two emails per hour. (Example: Sending four emails during a two-hour meeting would count as multitasking.)</li></ul>|Meeting|Count|Yes|
|Attendees with conflicting meeting|Number of attendees with meetings that overlap with the meeting (includes all non-declined meetings, which include accepted, tentative, and no responses to meeting invites).|Meeting|Count|Yes|
|Emails sent during meetings|Number of emails the person sent during all meetings.|Meeting|Count|Yes|
|Invitees|Number of people invited to the meeting.|Meeting|Count|Yes|
|Redundant attendees | The number of attendees of a meeting who are redundant, as defined by the _Redundant meeting hours (lower level)_ metric. For more information about _Redundant meeting hours (lower level)_, see the table that lists [Person metrics](#person-metrics).  |Meeting|Count|Yes|
|Total meeting cost|The total cost of all attendees in a meeting. The meeting cost for each attendee is defined as the product of the attendees' meeting hours multiplied by the attendees' hourly rates. If no hourly rate is available for one or more attendees, the default rate of $75/hr (US dollars) is used to calculate the cost of those attendees.|Meeting|Currency|Yes|
|Total redundant hours|The total number of redundant hours metric for all attendees in a meeting.|Meeting|Hour|Yes|

## Group-to-group metrics

|Metric|Description|Query type|Data type|Customizable|
|------|-----------|----------|---------|------------|
|Collaboration hours |Sum of meeting hours and email hours spent between the time investor and collaborator groups.|Group|Hour|No|
|Email hours |Number of hours spent sending and reading emails between the time investor and collaborator groups.|Group|Hour|No|
|Employees engaged |Number of people in the time investor's group who had two or more meaningful interactions in the last 28 days with the collaborator's group. This only counts licensed employees.​|Group|Count|No|
|LastTimeContacted|The last date and time that a person from the time investor's group emailed or attended a meeting with one or more people in the collaborator group for the specified date range. |Group|DateTime|No|
|Meeting attendee count|Total number of attendees in all meetings from the time investor and collaborator groups.|Group|Count|No|
|Meeting hours |Number of meeting hours the time investor group has spent meeting with the collaborator group.|Group|Hour|No|
|Meeting invitee count|Total number of invitees in all meetings from the time investor and collaborator groups.|Group|Count|No|
|Meetings |Number of distinct meetings with at least one attendee from the time investor and collaborator groups.|Group|Count|No|
|Network size|Number of people in the collaborator group who had at least two meaningful interactions in the last 28 days with the time investor's group. This only counts licensed employees. |Group|Count|No|
|Time investors initiated meeting hours | This calculates the number of meeting hours the time investors created only for *Internal collaborators* or *Collaborators within group* by organizing meetings. (Doesn’t follow time-allocation logic.)​ |Group|Hour|No|

## Person-to-group metrics

|Metric|Description|Query type|Data type|Customizable|
|------|-----------|----------|---------|------------|
|Collaboration hours|Total number of meeting and email hours for the time investor with one or more people in the collaborator group. This metric uses time allocation logic. |Group|Hour|No|
|Email count|Count of unique email exchanges (sent and received) that the time investor had with one or more people in the collaborator group. |Group|Count|No|
|Email hours|Total number of hours that the time investor spent sending and reading emails with one or more people in the collaborator group. This metric uses time allocation logic. |Group|Hour|No|
|LastTimeContacted |The last date and time that the time investor (measured employee) emailed or attended a meeting with one or more people in the collaborator group for the specified date range. |Group|DateTime|No|
|Meeting hours|Total number of hours that the time investor spent in meetings with one or more people in the collaborator group. This metric uses time allocation logic. |Group|Hour|No|
|Meetings|Number of unique meetings that the time investor attended with one or more people in the collaborator group. |Group|Count|No|
|Network size|Number of people in the collaborator group who had at least two meaningful interactions in the last 28 days with the time investor. This counts both licensed and unlicensed employees in the collaborator group. |Group|Count|No|
