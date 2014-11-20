Technicial data on Schools websites in England
=======================

A extract from [EduBase](http://www.education.gov.uk/edubase/home.xhtml) by [Department 
for Education](https://www.gov.uk/government/organisations/department-for-education) was taken on Nov-14.

The IPv6 scores was based on the [IPv6 health check](https://www.mythic-beasts.com/ipv6/health-check) by [Mythic Beasts](https://www.mythic-beasts.com/).

Domain registration look up was performed by using [WHOIS tool](http://www.nominet.org.uk/whois/) by [Nominet](http://www.nominet.org.uk/).

#### School_ID
Surrogate key
Field Type: integer
Data Source: Script
Notes: 

#### LaNumber
3 digit Local Authority number
Field Type: integer
Data Source: Edubase

#### EstablishmentNumber
4 digit Establishment (school) number
Field Type: integer
Data Source: Edubase

#### LA
Local Authority name
Field Type: string
Data Source: Edubase
Notes:

#### Establishment
Establishment (school) name
Field Type: string
Data Source: Edubase
Notes:

#### WebSiteAddress
Establishment (school) website url (including protocol)
Field Type: string
Data Source: Edubase
Notes: Minor data cleansing

#### Size
Disc size of raw HTML code for Establishment (school) website homepage in bytes
Field Type: integer
Data Source: HTML request
Notes:

#### GoogleAnalytics
If the raw HTML code for Establishment (school) website homepage contains the Google Analytics javascript
Field Type: boolean
Data Source: HTML request
Notes:

#### IE6Support
If the raw HTML code for Establishment (school) website homepage appears to contains a specific Internet Explorer 6.0 workaround.
Field Type: boolean
Data Source: HTML request
Notes:

#### DomainName
Establishment (school) domain based on the website address
Field Type: string
Data Source: Edubase
Notes: Scripted

#### RegisteredOwner
The registered owner of the domain
Field Type: string
Data Source: Nominet
Notes: Only .UK domains.
