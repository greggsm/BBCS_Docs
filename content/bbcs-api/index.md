---
layout: layout-sidebar
order: 3
name: BBCS API
description: render side navigation on the left hand side of the page using H2 tags
published: true
showInNav: true
showInHeader: true
showInFooter: true
---


# BBCS API Documentation #

## Introduction 

This page demonstrates how to use the BBCS API endpoints.

## BBInvoker Settings

Setting up BBInvoker for testing email.

## REST Endpoints

### Admin
- Client
- Get
- Ping 

### Status
- Job
- Blacklist
- Recipient
- Ping

### Submission
- Bulk
- BulkCreate
- BulkAddData
- BulkProcess
- Transactional
- Ping


## SOAP Endpoints

### Email Status Service
WCF Service that exposes methods to get status information on email jobs and email recipients.

- DeactivateEmailBlacklist Method: 
- GetEmailJobStatus Method: 
- GetEmailRecipientStatus Method: 
- GetGeneralPurposeEmailJobStatus Method: 
- GetGeneralPurposeEmailJobStatusByID Method: 
- GetGeneralPurposeEmailRecipientStatus Method: 
- GetHardBounceRecipientStatus Method: 
- GetTransactionalEmailJobStatus Method: 
- GetTransactionalEmailJobStatusByID Method: 
- GetTransactionalEmailRecipientStatus Method: 
- Ping Method: 

### Email Submission Service
This service is used to submit transactional and general purpose email jobs. General purpose jobs can be submitted as a complete job, or in chunks depending on job size. All jobs enter the BBCS system through the submission service.

- SubmitGeneralPurposeEmailJob Method: 
- StartChunkedGeneralPurposeEmailJob Method: 
- SubmitGeneralPurposeEmailChunk Method: 
- EndChunkedGeneralPurposeEmailJob Method: 
- SubmitTransactionalEmailJob Method: 
- Ping Method: 