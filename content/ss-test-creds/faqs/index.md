---
layout: layout-sidebar
order: 
name: Email FAQs
description: render side navigation on the left hand side of the page using H2 tags
published: true
showInNav: true
showInHeader: true
showInFooter: true
---


# Email FAQs

## Where the *#@! is my email?
Assuming you've checked your application and environment for any submission errors, please allow for a reasonable amount of time to process before escalation. Our test environments are shared by multiple teams and depending on many variables, processing times can vary. If you need assistance with errors associated with our email systems, or have given a reasonble time for delivery of email, you can contact Gregg Smith or anyone on the Shared Services QA team for assistance. Please ensure your credentials are correct by reviewing our email test credentials page.

Also, please note that our QA and DEV environments are restricted to blackbaud.com, blackbaud.uk.co and blackbaud.au. All other domains are blocked at the firewall.


## What is the latest production version of Shelby Services and where can I find it on the network?

Shelby Services 6.0.92.0, deployed on 12/09/14, is the current production version. It can be found at \\ntcdl\apps\bbnc\Services\Build6.0.92.0.


## Where can I find status code information?

Always verify with your own team in case there are application changes in your version. However, we do list this information in our Services Troubleshooting Cheat Sheet.


I am getting an error in my BBNC TestConfig for the BBNC Service. Any ideas?

Try our Services Troubleshooting Cheat Sheet after contacting the Fundraising or Platform teams.


## Where can I find design information on the new client-side email services?

Please consult this document for client-side email services design and API.


## Any API documentation?

Yep.


## How can I ensure my client data contains no pending emails?

It is recommended to always check with your engineering manager/team to ensure you have the latest information and best practices. Many teams run this against their client databases before integrating with our test mail systems.


## What is BBCS?

Blackbaud Communication Services (BBCS) is our application that handles the tranferring of email job information (successfull and bounced email) from StrongMail to Shelby Services. This is done via a series of global changes. It soon will become the replacement to the Shelby Services' Services Administrator.


## What is the latest production version of BBCS?

BBCS 4.0.63.0, deployed on 06/19/16, is the current production version.


## How can I test email bounces?

Check out Gregg Smith's blog post on how to do this with BBInvoker.


## Why am I not getting emails sent to non-blackbaud domains (e.g. gmail, hotmail, etc.)? How can I send to another domain?

Our QA test environment is locked down at the firewall to prevent outbound email. This was put in place due to overwhelming demand to restrict accidental exposure of email addresses. Deliverability outside of blackbaud.com should not be a test concern.  This rule cannot be suspended.

It is possible to send email to another internal email address other than @blackbaud.com by creating a phony domain. If this is a need, please contact Scott Carnley or Gregg Smith. Each request will be evaluated on a case by case basis.


## Can I run load tests in the test environments?

No. This email test environment is not a load test environments. Email load testing is performed by the Shared Services team. If you need to run a load test, please contact Jason Na or Scott Carnley.


## What is the resend policy for soft bounced emails?

By default, the initial retry interval is 900 seconds, and the deferred message expiration time is 28,000 seconds. This means the first retry of a deferred message will be 15 minutes after it is deferred. Subsequent retries will take place at 30 minutes, 1 hour, 2 hours, 4 hours, and 8 hours. After the expiration time of 8 hours, a retry will result in a permanent failure.

Soft bounces are bounced emails caused by a temporary failure such as a network error, full mailbox, or content filter. Hard bounces, such as a bad domain name, result in automatic failure and will not be retried.