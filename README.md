# cofi-public-data

This repo contains publicly available data in support of CoFi services development and deployment.

The first such data set concerns the city of Lancaster and surrounding area. It consists of geolocated company mapping data obtained from the public [UK Companies House](https://www.gov.uk/government/organisations/companies-house) database.

The data was constructed by first selecting the [District postcodes](https://en.wikipedia.org/wiki/Postcodes_in_the_United_Kingdom) of Lancaster (LA1 to LA7) from [Doogal](https://www.doogal.co.uk/Counties?county=E10000017) and then filtering all the CH companies that fall within these 7 postcode districts. The Doogal data includes GPS coordinates for each Unit postcode.

The CH records contain also the UK Standard Industry Classification (SIC 2007) code for each company. After generating a custom colour code for the 88 SIC Divisions (business sectors), a tally of the filtered companies over these divisions was calculated.

Finally, Mathematica was used to generate 84 maps, where each map visualises the companies belonging to the corrosponding division as a set of points coloured with the colour maps and geolocated using the GPS coordinates corresponding to its Unit postcode.
