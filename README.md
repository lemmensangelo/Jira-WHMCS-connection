# Jira WHMCS connection

## Features
- Redirects admins/clients to Jira Service Desk in case they click on view ticket(s) or after the creation of a ticket in Jira.
- If client or admin stil manages to create a ticket through WHMCS the ticket will be send to Jira and be deleted in WHMCS.

## Installation
1. Dowload and unzip this in your WHMCS installation in the folder `modules/addons`.
2. Activate the module in module settings.
3. Click on `Configure`
4. Enter all the details.
> NOTE 
>
> If you don't know you Jira Service Desk ID or Jira Request Type ID fill in your Jira email and Jira API KEY
> Then go to Module -> jira Extension
> Click on either `View my Jira Service Desks` or `View my Jira Request Types`
> This page will show you alle the ID's needed.
5. Go to Modules -> Jira Extension to see if the status of the Jira Extension is all green.
6. Your all set up now.

> IMPORTANT 
>
> If you enable Jira Extension please make sure in `Email Templates` all support emails are turned off so your clients won't get emails from WHMCS.

## Options
There are 4 main function you can choose.
1. Redirect admins (State Admin Redirect)
2. Redirect clients (State Customer Redirect)
3. Send ticket to Jira (State Create Ticket)
4. Delete ticket after send to Jira (State Delete Tickets)

These can't be cosumized through the module but can be changed in the database in the table `mod_jiraextension`.
