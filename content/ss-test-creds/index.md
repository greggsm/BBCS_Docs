---
layout: layout-sidebar
order: 2
name: Email Test Credentials
description: render side navigation on the left hand side of the page using H2 tags
published: true
showInNav: true
showInHeader: true
showInFooter: true
---


# Shared Services QA Production Email Test Environment Credentials #

Disclaimer: These environments are for internal use only. They are not to be distributed to clients. Please DO NOT load test email on these environments.
Service alerts and status information can be found on our Home page. BBPS, BBMS, and BBSP test credentials are here.
 
Looking for development or load testing environments? Contact Gregg Smith, Jason Na or a member of the Shared Services team for assistance.


## Connecting to Blackbaud Communication Services (BBCS)

The Shared Services QA Production Email Test Environment uses only BBCS to process email and publish status so if you need services particular to Shelby Services such Email forwarding or CapWiz please contact Gregg Smith, Jason Na or a member of the Shared Services team for assistance.

### Email Service Settings

<p>Host: bbcs-service.sharedservices-dev.com</p>
<p>User name: {USERNAME}</p>
<p>Use SSL: Yes</p>
<p>Password: adminadmin_2</p>

## Test Organization Usernames and Passwords

Do you really need to test full deliverability? In most cases, you simply need email services to accept your email job. The following account will accept all email jobs, but not process them.


<div class="table-responsive">
  <table class="table table-striped table-hover">
    <thead>
        <tr>
            <th>Team</th>
            <th>Username</th>
            <th>Password</th>
        </tr>
    </thead>
    <tbody>
    <tr>
        <td>Any team</td>
        <td>acceptonly</td>
        <td>adminadmin_2</td>
    </tr>
    </tbody>
  </table>
</div>

If you need email to be sent to your blackbaud.com email address, you may use the following accounts. Do not load test against these environments, nor send up large email jobs. Client databases should have their email addresses scrubbed and pending email jobs cleared before integrating.

<div class="table-responsive">
  <table class="table table-striped table-hover">
    <thead>
        <tr>
            <th>Team</th>
            <th>Username</th>
            <th>Password</th>
        </tr>
    </thead>
    <tbody>
    <tr>
        <td>Altru</td>
        <td>altru</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>BBOX</td>
        <td>BBOX</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Cambridge</td>
        <td>cambridge</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Classics</td>
        <td>classics</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Corp IT</td>
        <td>CorporateIT</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Enterprise</td>
        <td>enterprise</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Financial</td>
        <td>financial</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Fundraising</td>
        <td>fundraising</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Internal Systems</td>
        <td>DemoUser</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Internet Solutions</td>
        <td>internetsolutions</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Luminate Online</td>
        <td>luminate</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>MicroEdge</td>
        <td>MicroEdge</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Online Express</td>
        <td>OXuser</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Platform</td>
        <td>platform</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Professional Services</td>
        <td>proservices</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Sales</td>
        <td>sales</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>San Diego</td>
        <td>sandiego</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>SD PaymentSupport</td>
        <td>SDPaymentSupport</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Support</td>
        <td>support</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>Verticals</td>
        <td>verticals</td>
        <td>adminadmin_2</td>
    </tr>
        <tr>
        <td>UK Support</td>
        <td>uksupport</td>
        <td>adminadmin_2</td>
    </tr>
    </tbody>
  </table>
</div>

If you need to test email bounces, please refer to our WIKI for information.
For issues with our QA Production Email Test Environment contact Gregg Smith, Jason Na or a member of the Shared Services team for assistance.


## BBInvoker Settings

Setting up BBInvoker for testing email.

