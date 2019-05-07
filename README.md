# ![LOGO](logo.png) Solar VPS **flow**ground Connector

## Description

A generated **flow**ground connector for the Solar VPS API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/solarvps.com/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:44:08+03:00

## API Description

This is the Solar VPS Public API. You can find more at http://www.solarvps.com

## Authorization

Supported authorization schemes:
- API Key
## Actions

### View all contacts under your account

> Shows all contacts under the client account.

*Tags:* `contacts`

### View all your records for a given domain

> Shows all your records for a specific domain. You can try example.com below.

*Tags:* `dns`

#### Input Parameters
* `domain` - _required_ - Domain name you want to get records for

### Add dns record for given domain

> You can try example.com below. Types allowed are: A CNAME NS TXT MX SRV SPF

*Tags:* `dns`

#### Input Parameters
* `domain` - _required_ - Domain you want to add records for
* `name` - _required_ - Fully qualified DNS name
* `type` - _required_ - Type of DNS record
* `content` - _required_ - Content for DNS record
* `ttl` - _required_ - Time To Live for DNS record
* `prio` - _required_ - Priority of DNS record

### Delete dns record for a given domain

> Shows all your records for a specific domain. You can try example.com below.

*Tags:* `dns`

#### Input Parameters
* `domain` - _required_ - Domain name you want to get records for
* `id` - _required_ - Id of the DNS Record

### Update dns record for a given domain

> You can try example.com below.

*Tags:* `dns`

#### Input Parameters
* `domain` - _required_ - Domain name to add record under
* `id` - _required_ - Id of DNS record
* `name` - _optional_ - Fully qualified name for the DNS record
* `type` - _optional_ - Type for DNS record
* `content` - _optional_ - Content for the DNS Record
* `ttl` - _optional_ - Time To Live for DNS record
* `prio` - _optional_ - Priority of the DNS record

### View all your domains managed by SolarVPS Distributed DNS

> Shows all your domains

*Tags:* `domains`

### Add domain to be managed by SolarVPS Distributed DNS

> Adds domain to SolarVPS Distributed DNS

*Tags:* `domains`

#### Input Parameters
* `domain` - _required_ - Domain to add to SolarVPS Distributed DNS

### Delete domain from SolarVPS Distributed DNS

> Deletes domain from SolarVPS Distributed DNS

*Tags:* `domains`

#### Input Parameters
* `domain` - _required_ - Domain to delete from SolarVPS Distributed DNS

### Generate API Key

> API Key is regenerated if it already exists

*Tags:* `key`

#### Input Parameters
* `username` - _required_ - Email address used to login to SolarSystem
* `password` - _required_ - Password used to login to SolarSystem

### Get API Key

> Gets the API Key for user

*Tags:* `key`

#### Input Parameters
* `username` - _required_ - Email address used to login to SolarSystem
* `password` - _required_ - Password used to login to SolarSystem

### View all your pods

> Shows all your pods

*Tags:* `pods`

### View information on a specific pod

> Shows details of a specific pod. Enter 1 below to see an example

*Tags:* `pods`

#### Input Parameters
* `podId` - _required_ - Id of the pod you want to perform actions on

### Ping your specified pod

> Returns the ping response from your server.

*Tags:* `pods`

#### Input Parameters
* `podId` - _required_ - Id of the pod you want to ping check

### Perform action on a specific pod

> Allowed actions are reboot, shutdown, boot

*Tags:* `pods`

#### Input Parameters
* `podId` - _required_ - Id of the pod you want to perform actions on
* `action` - _required_ - Action to perform on selected pod

### View all your monitors

> Shows all your monitors

*Tags:* `solarray`

### View all your critical notifications

> Shows all your critical notifications

*Tags:* `solarray`

### View all your tickets

> Shows all your tickets

*Tags:* `tickets`

### Open ticket with desired department

> Available departments are support, billing, sales

*Tags:* `tickets`

#### Input Parameters
* `department` - _required_ - Department you want to open a ticket with
* `subject` - _required_ - Subject of the ticket you are opening
* `contents` - _required_ - Message reply being sent

### View details on a specific ticket

> Shows all information of a specific ticketId

*Tags:* `tickets`

#### Input Parameters
* `ticketId` - _required_ - TicketId you want to see

### Post a reply to a ticket

*Tags:* `tickets`

#### Input Parameters
* `ticketid` - _required_ - TicketId of the ticket you want to post an update to
* `contents` - _required_ - Message reply being sent

## License

**flow**ground :- Telekom iPaaS / solarvps-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
