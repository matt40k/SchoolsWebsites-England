# Technical data on Schools websites in England

A extract from [EduBase](http://www.education.gov.uk/edubase/home.xhtml) by [Department 
for Education](https://www.gov.uk/government/organisations/department-for-education) was taken on Nov-14.

The IPv6 scores was based on the [IPv6 health check](https://www.mythic-beasts.com/ipv6/health-check) by [Mythic Beasts](https://www.mythic-beasts.com/).

Domain registration look up was performed by using [WHOIS tool](http://www.nominet.org.uk/whois/) by [Nominet](http://www.nominet.org.uk/).

### Tools used
* Microsoft Excel
* Microsoft SQL Server
* PowerShell
* Visual Studio (C#)

## Data fields

#### School_ID
Surrogate key.

Field Type: integer

Data Source: Script

Notes: 

#### LaNumber
3 digit Local Authority number.

Field Type: integer

Data Source: Edubase

Notes: 

#### EstablishmentNumber
4 digit Establishment (school) number.

Field Type: integer

Data Source: Edubase

Notes: 


#### LA
Local Authority name.

Field Type: string

Data Source: Edubase

Notes:

#### Establishment
Establishment (school) name.

Field Type: string

Data Source: Edubase

Notes:

#### WebSiteAddress
Establishment (school) website url (including protocol).

Field Type: string

Data Source: Edubase

Notes: Minor data cleansing

#### Size
Disc size of raw HTML code for Establishment (school) website homepage in bytes.

Field Type: integer

Data Source: HTML request

Notes:

#### GoogleAnalytics
If the raw HTML code for Establishment (school) website homepage contains the Google Analytics javascript.

Field Type: boolean

Data Source: HTML request

Notes:

#### IE6Support
If the raw HTML code for Establishment (school) website homepage appears to contains a specific Internet Explorer 6.0 workaround.

Field Type: boolean

Data Source: HTML request

Notes:


#### DomainName
Establishment (school) domain based on the website address.

Field Type: string

Data Source: Edubase

Notes: Scripted

#### RegisteredOwner
The registered owner of the domain.

Field Type: string

Data Source: Nominet

Notes: Only .UK domains.

#### RegisteredOwnerType
The Nominet defined domain owner type - UK School \ UK Individual \ etc.

Field Type: string

Data Source: Nominet

Notes: Only .UK domains.

#### Registrar
The registrar who the establishment (school) has registered the domain via.

Field Type: string

Data Source: Nominet

Notes: Only .UK domains.

#### GoldenRegistrar
If the registrar has 100% success rate at correctly registering **all** domains. The registered owner type **must** be UK School.

Field Type: boolean

Data Source: Script

Notes: Only .UK domains.

#### RegistrarSchoolCount
The number of schools the registrator has registered (in this extract).

Field Type: integer

Data Source: Nominet

Notes: Only .UK domains.

#### CMS
Uses the meta tag generator from the raw HTML code for Establishment (school) website homepage to determine the CMS used (if any).

Field Type: string

Data Source: HTML request

Notes:

#### HTMLtype
Uses the HTML type from the raw HTML code for Establishment (school) website homepage.

Field Type: string

Data Source: HTML request

Notes:


#### IPv6Score
Uses the Mythic Beasts IPv6 Health checker scoring out of 9.

Field Type: integer

Data Source: Mythic Beasts IPv6 Health checker

Notes:


#### UKDomain
If the establishment (school) website is a .UK domain.

Field Type: boolean

Data Source: Script

Notes:


#### PostCode
Establishment (school) post code.

Field Type: string

Data Source: EduBase

Notes:

#### Easting
Establishment (school) post code.

Field Type: string

Data Source: EduBase

Notes:

#### Northing
Establishment (school) post code.

Field Type: string

Data Source: EduBase

Notes:

#### HeadName
Establishment (school) HeadTeacher name.

Field Type: string

Data Source: EduBase

Notes: concatenate from Head's title, first letter of the forename and surname.


