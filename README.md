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

Column | Type | Data Source
--- | --- | ---
School_ID | integer | Script
LaNumber | integer | [EduBase](http://www.education.gov.uk/edubase/home.xhtml)
EstablishmentNumber | integer | [EduBase](http://www.education.gov.uk/edubase/home.xhtml)
LA | string | [EduBase](http://www.education.gov.uk/edubase/home.xhtml)
Establishment | string | [EduBase](http://www.education.gov.uk/edubase/home.xhtml)
WebSiteAddress | string | [EduBase](http://www.education.gov.uk/edubase/home.xhtml)
Size | integer | HTML request
GoogleAnalytics | boolean | HTML request
IE6Support | boolean | HTML request
DomainName | string | [EduBase](http://www.education.gov.uk/edubase/home.xhtml)
RegisteredOwner | string | [Nominet](http://www.nominet.org.uk)
RegisteredOwnerType | string | [Nominet](http://www.nominet.org.uk)
Registrar | string | [Nominet](http://www.nominet.org.uk)
GoldenRegistrar | boolean | Script
RegistrarSchoolCount | integer | [Nominet](http://www.nominet.org.uk)
CMS | string | HTML request
HTMLtype | string | HTML request
IPv6Score | integer | [Mythic Beasts](https://www.mythic-beasts.com/) [IPv6 Health checker](https://www.mythic-beasts.com/ipv6/health-check)
UKDomain | boolean | Script
PostCode | string | [EduBase](http://www.education.gov.uk/edubase/home.xhtml)
Easting | integer| [EduBase](http://www.education.gov.uk/edubase/home.xhtml)
Northing | integer| [EduBase](http://www.education.gov.uk/edubase/home.xhtml)
HeadName | string | [EduBase](http://www.education.gov.uk/edubase/home.xhtml)

### Descriptions

#### School_ID
Surrogate key.

#### LaNumber
3 digit Local Authority number.

#### EstablishmentNumber
4 digit Establishment (school) number.

#### LA
Local Authority name.

#### Establishment
Establishment (school) name.

#### WebSiteAddress
Establishment (school) website url (including protocol).

Notes: Minor data cleansing

#### Size
Disc size of raw HTML code for Establishment (school) website homepage in bytes.

#### GoogleAnalytics
If the raw HTML code for Establishment (school) website homepage contains the Google Analytics javascript.

#### IE6Support
If the raw HTML code for Establishment (school) website homepage appears to contains a specific Internet Explorer 6.0 workaround.

#### DomainName
Establishment (school) domain based on the website address.

#### RegisteredOwner
The registered owner of the domain.

Notes: Only .UK domains.

#### RegisteredOwnerType
The Nominet defined domain owner type - UK School \ UK Individual \ etc.

Notes: Only .UK domains.

#### Registrar
The registrar who the establishment (school) has registered the domain via.

Notes: Only .UK domains.

#### GoldenRegistrar
If the registrar has 100% success rate at correctly registering **all** domains. The registered owner type **must** be UK School.

Notes: Only .UK domains.

#### RegistrarSchoolCount
The number of schools the registrator has registered (in this extract).

Notes: Only .UK domains.

#### CMS
Uses the meta tag generator from the raw HTML code for Establishment (school) website homepage to determine the CMS used (if any).

#### HTMLtype
Uses the HTML type from the raw HTML code for Establishment (school) website homepage.

#### IPv6Score
Uses the Mythic Beasts IPv6 Health checker scoring out of 9.

#### UKDomain
If the establishment (school) website is a .UK domain.

#### PostCode
Establishment (school) post code.

#### Easting
Establishment (school) post code.

#### Northing
Establishment (school) post code.

#### HeadName
Establishment (school) HeadTeacher name.

Notes: concatenate from Head's title, first letter of the forename and surname.


