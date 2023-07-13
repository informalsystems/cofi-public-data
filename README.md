# cofi-public-data

This repo contains publicly available data in support of CoFi services development and deployment.

The first such data set concerns the city of Lancaster and surrounding area. It consists of geolocated company mapping data obtained from the public [UK Companies House](https://www.gov.uk/government/organisations/companies-house) database. There are 85 out of 88 maps because 3 divisions are absent from Lancaster: 5, 19, and 21.

The second data set covers Merseyside, including the Wirral, and consists of 88 maps (all sectors are represented).

The data was constructed by first selecting the [District postcodes](https://en.wikipedia.org/wiki/Postcodes_in_the_United_Kingdom) of Lancaster (LA1 to LA7) from [Doogal](https://www.doogal.co.uk/Counties?county=E10000017) and then filtering all the CH companies that fall within these 7 postcode districts. The Doogal data includes GPS coordinates for each Unit postcode.

In the case of Merseyside, the following postcode areas and sectors were mapped:
L1,L2,L3,L4,L5,L6,L7,L8,L9,L10,L11,L12,L13,L14,L15,L16,L17,L18,L19,L20,
L21,L22,L23,L24,L25,L26,L27,L28,L29,L30,L31,L32,L33,L34,L35,L36,L37,L38,L39,
L67,L68,L69,L70,L71,L72,L74,L75,L80,PR8,PR9,
CH25,CH26,CH27,CH28,CH29,CH30,CH31,CH32,CH41,CH42,CH43,CH44,CH45,CH46,CH47,CH48,CH49,
CH60,CH61,CH62,CH63,CH64,CH65,WA2,WA3,WA5,WN4,WN5,WA8,WA9,WA10,WA11,WA12
Some of these are actually PO Boxes rather than geographical postcodes, but they still have a geographical location at a specific post office.

The CH records contain also the UK Standard Industry Classification (SIC 2007) code for each company. After generating a custom colour code for the 88 SIC Divisions (business sectors), a tally (distribution) was calculated by filtering the companies over these divisions.

Finally, Mathematica was used to generate the maps, where each map visualises the companies belonging to the corrosponding division as a set of points coloured with the colour maps and geolocated using the GPS coordinates corresponding to its Unit postcode.

(The Doogal and the Companies House data is released under the [Open Government Licence v.3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).) 
