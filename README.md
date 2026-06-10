# Khandie Gym — Member Lifecycle & Renewal System

An end-to-end membership management system that automates 
enrollment, expiry tracking, and renewal reminders for a gym 
business — replacing manual follow-ups entirely.

## Problem It Solves
The gym was manually tracking member subscriptions in 
spreadsheets, missing renewal dates, and losing members 
due to lack of timely follow-up.

## Tools Used
- n8n (workflow automation)
- Airtable (member database)
- Tally (enrollment form)
- Email (automated notifications)

## How It Works
1. New member submits Tally enrollment form
2. n8n captures submission and creates a record in Airtable
   with membership start and calculated expiry date
3. Scheduled trigger checks Airtable daily for expiring memberships
4. Members approaching expiry receive automated reminder emails
5. On renewal, membership dates are updated automatically in Airtable

## Key Concepts Demonstrated
- Tally form → n8n → Airtable pipeline
- Luxon date expressions for expiry calculation
- Scheduled workflow triggers
- Airtable typecast for date fields
