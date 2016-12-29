<h3>Do you support the MySQL extension in PHP, or just the MySQLi extension?</h3>

For security reasons DomainMOD only supports the MySQLi extension. If you're receiving messages that the MySQLi extension is unavailable, you will need to install and enable it on your server before you can use DomainMOD.


<BR><h3>Does DomainMOD support multiple languages?</h3>

Currently only English is supported, but this is something that will be investigated for the future.


<BR><h3>How many domains can I manage with DomainMOD?</h3>

Theoretically there's no limit on the number of domains you can manage, it just depends on your server hardware and the settings chosen in DomainMOD. The default settings can handle thousands of domains, and over 10,000 depending on how much information you've chosen to display on the front page, but if things start slowing down you can enable "large mode" to speed things up. Large mode uses a different method for displaying the information on the main domain page, and although it doesn't offer as many of the advances features as the default settings, it allows you to manage a lot more domains.


<BR><h3>Can I import my domains into DomainMOD using a CSV file?</h3>

Not currently, but this is something that we're investigating for the future. If your domain registrar has an API, and it's [supported by DomainMOD](domain-queue.md#supported-registrars), you can use the [Domain Queue](domain-queue.md) to automatically import your domains.


<BR><h3>Which domain registrar APIs does DomainMOD currently support?</h3>

DomainMOD currently supports DNSimple, Dynadot, eNom, Fabulous, GoDaddy, Internet.bs, Name.com, NameBright, Namecheap, NameSilo, OpenSRS, and ResellerClub.


<BR><h3>Are the domain expiration dates updated automatically using the domain's WHOIS information?</h3> 

No, expiration dates currently need to be updated manually when the domains are renewed.


<BR><h3>Can I use DomainMOD to sell domains?</h3>

The primary use for DomainMOD is to manage a large portfolio of domains, and it currently doesn't have any sales features, such as being able to host sales letter landing pages. This is something we're looking at implementing in a future version of DomainMOD.

If all you want to do is track the amount you sold a domain for, you can create a Custom Field, which will allow you to record the sales amount for your domains.


<BR><h3>I noticed you can set the registration, transfer, and renewal prices for domains via their domain registrars, but can you set a purchase price for a specific domain? For example, if I purchase a domain from a 3rd party marketplace can I record this information in DomainMOD?</h3>

Although purchase price is not a standard field, you can use [Custom Fields](administration.md#custom-fields) to keep track of the purchase prices for your domains.


<BR><h3>I don't need to keep track of the fees associated with my domains. Can I disable this feature?</h3>

There's currently no way to disable fees, as the system requires them in order to link the database tables, but if you don't care about keeping track of the fees you can just enter zeros for all of the costs.


<BR><h3>Something else</h3>

