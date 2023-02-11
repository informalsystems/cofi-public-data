# cofi-public-data

This repo contains publicly available data in support of CoFi services development and deployment.

The first such data set concerns the city of Lancaster and surrounding area. It consists of geolocated company mapping data obtained from the public [UK Companies House](https://www.gov.uk/government/organisations/companies-house) database.

The data was constructed by first selecting the [District postcodes](https://en.wikipedia.org/wiki/Postcodes_in_the_United_Kingdom) of Lancaster (LA1 to LA7) from [Doogal](https://www.doogal.co.uk/Counties?county=E10000017) and then filtering all the CH companies that fall within these 7 postcode districts. The Doogal data includes GPS coordinates for each Unit postcode.

The CH records contain also the UK Standard Industry Classification (SIC 2007) code for each company. After generating a custom colour code for the 88 SIC Divisions (business sectors), a tally (distribution) was calculated by filtering the companies over these divisions.

Finally, Mathematica was used to generate 85 maps, where each map visualises the companies belonging to the corrosponding division as a set of points coloured with the colour maps and geolocated using the GPS coordinates corresponding to its Unit postcode. There are only 85 maps because 3 Divisions are not present in the Lancaster region: 5, 19, and 21.

(The Doogal and the Companies House data is released under the [Open Government Licence v.3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).) 
