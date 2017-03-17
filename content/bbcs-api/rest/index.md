---
layout: layout-sidebar
order: 2
name: REST Endpoints
description: render side navigation on the left hand side of the page using H2 tags
published: true
showInNav: true
showInHeader: true
showInFooter: true
---


# BBCS REST API Documentation #

## Introduction 

This page demonstrates how to use the BBCS API endpoints.

## REST Endpoints

### Admin
- Client
    - Adds a new sub-client record to the Blackbaud Communication Service.    
- Get
    - Retrieves the details for a sub-client record.   
- Ping 
    - Pings the service to check for a successful connection.

### Status
- Job
    - Requests a compressed data set of email jobs.
- Blacklist
    - Removes the supplied email address from the blacklist for the calling organization.
- Recipient
    - Requests a compressed data set of recipient bounces.
- Ping
    - Pings the service to check for a successful connection.

### Submission
- Bulk
    - Creates and processes a bulk email job
- BulkCreate
    - Creates a bulk email job.
- BulkAddData
    - Adds data to an existing bulk email job that has not yet begun processing.
- BulkProcess
    - Starts processing on a bulk email job that was created with BulkCreate.
- Transactional
    - Creates and processes a transactional email job.
- Ping
    - Pings the service to check for a successful connection.
