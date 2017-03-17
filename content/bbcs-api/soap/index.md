---
layout: layout-sidebar
order: 3
name: SOAP Endpoints
description: render side navigation on the left hand side of the page using H2 tags
published: true
showInNav: true
showInHeader: true
showInFooter: true
---

# BBCS SOAP API Documentation #
## Introduction 
This page demonstrates how to use the BBCS API endpoints.
## SOAP Endpoints
### Email Status Service
WCF Service that exposes methods to get status information on email jobs and email recipients.

- DeactivateEmailBlacklist Method: 
    - Deactivates a blacklist flag on a spam complaint or hard bounce for the provided email address.
- GetEmailJobStatus Method: 
    - Returns the status of any email jobs after the specified date for the calling organization.
- GetEmailRecipientStatus Method: 
    - Return the records of any bounced emails after the specified date for the calling organization.
- GetGeneralPurposeEmailJobStatus Method: 
    - Returns the status of any general purpose email jobs after the specified date for the calling organization.
- GetGeneralPurposeEmailJobStatusByID Method: 
    - Returns the status of the specified general purpose email job.
- GetGeneralPurposeEmailRecipientStatus Method: 
    - Return the records of any bounced general purpose emails after the specified date for the calling organization.
- GetHardBounceRecipientStatus Method: 
    - Return the records of any hard bounced emails after the specified date for the calling organization.
- GetTransactionalEmailJobStatus Method: 
    - Returns the status of any transactional email jobs after the specified date for the calling organization.
- GetTransactionalEmailJobStatusByID Method: 
    - Returns the status of the specified transactional email job.
- GetTransactionalEmailRecipientStatus Method: 
    - Return the records of any bounced transactional emails after the specified date for the calling organization.
- Ping Method: 
    - Pings the status service to see if it is currently running.

### Email Submission Service
This service is used to submit transactional and general purpose email jobs. General purpose jobs can be submitted as a complete job, or in chunks depending on job size. All jobs enter the BBCS system through the submission service.

- SubmitGeneralPurposeEmailJob Method: 
    - Loads and records the job template and merge data. Indicates that the job is ready to submit to the MTAs. Only used with jobs that do not contain enough merge data to require chunking.
- StartChunkedGeneralPurposeEmailJob Method: 
    - Loads and records the job template and first chunk of merge data. Does not submit any data to the MTAs.
- SubmitGeneralPurposeEmailChunk Method: 
    - Submits a chunk of merge data associated with a pre-existing job. Does not submit any data to the MTAs.
- EndChunkedGeneralPurposeEmailJob Method: 
    - Indicates that the specified job is ready to be sent to strongmail.
- SubmitTransactionalEmailJob Method: 
    - Loads and records the job template and merge data. Indicates that the job is ready to submit to the MTAs. A transactional job is an acknowledgment of a user action, can only contain one recipient, and does not respect spam complaints.
- Ping Method: 
    - Pings the submission service to see if it is currently running.