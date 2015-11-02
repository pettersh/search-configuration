# SharePoint Search Configurations
By *Petter Skodvin-Hvammen - [Principal Consultant at Puzzlepart](http://www.puzzlepart.com)*

## Enable Content Source

ContentSource is a managed property that contains the name of the content source used to crawl the current item. The managed property is populated by SharePoint using a hidden crawled property named 315 from the Internal category. You cannot change system provided managed properties in SharePoint Online, but you can change mappings and provide an alias. 

Kudos and credits to my colleague **Mikael Svenson** for his blog post [Debug crawled properties and creating a refiner for Content Source without modifying the existing ContentSource managed property](http://techmikael.blogspot.no/2014/09/debug-crawled-properties-and-creating.html)

You can import the search configurations files to your SharePoint Online schema at the tentant level from https://contoso-admin.sharepoint.com/_layouts/15/searchadmin/importsearchconfiguration.aspx?level=tenant

- *ContentSource-315-Internal_CP_MP_Mapping_Alias.xml*
-- Create the crawled property *Internal:315*, map to *RefinableString00* managed property and define *Source* as alias for tha managed property.
- *ContentSource-315-Internal_CP_Only.xml*
-- Create the crawled property *Internal:315*, map to *RefinableString00* managed property and define *Source* as alias for tha managed property.

## Follow me on 

- Twitter: [@pettersh](https://twitter.com/pettersh)
- My blog: (https://skodvinhvammen.wordpress.com)
- LinkedIn: (https://no.linkedin.com/in/petterskodvin)


