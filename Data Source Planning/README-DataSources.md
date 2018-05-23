# ATX-Displacement-Alert

## Summary of Solution
We are looking to create an interactive map web application, with multiple layers overlayed on the map to describe the risk of resident/tenant displacement. Because the real-time eviction filings provide only zip code level data and represent only a part of all displacements, we have sought to use multiple data sources that provide both a higher level of resolution (i.e. we want data that is localized on areas smaller than zip code level) and a more complete sketch of the factors that correlate with displacement.

## Overview of Data sources
Currently, we aim to describe the risk of displacement using the following risk factors:
1. recent eviction filings (zip code resolution)
2. new building sales (street address resolution)
3. new building construction permits (street address resolution)
                        +
4. eviction rates from 2000-2016 (block group resolution).
5. poverty rates from 2000-2016 (block group resolution).
6. median property value from 2000-2016 (block group resolution).
7. percent renter occupied from 2000-2016 (block group resolution).
8. population size from 2000-2016 (block group resolution).

## Detailed Description of Data sources
1. recent eviction filings (zip code resolution)
    * This factor consists of eviction hearing records on the Travis County Court Docket.
    - [x] The data source that provides up-to-date localized data has been identified.
        * This data originates from dynamically generated webpages on this website: https://odysseypa.tylerhost.net/Travis/default.aspx
        * The data can be accessed by the following navigation on the above website:
            A. Select "Court Calendar".
            B. On new page, select "Date Range", then deselect all case categories other than "Civil".
            C. Select desired date range.
    - [ ] This data is ready for incorporation into an experimental database.
    - [ ] Services have been prepared to regularly update this data source into database.
2. new building sales (street address resolution)
    * This factor consists possibly of either recent home sales in Travis County, or homes on market in Austin.
    - [ ] The data source that provides up-to-date localized data has been identified.
        * Some examples of almost sufficient data sources include: http://www.austinhomesearch.com/Listing/ListingSearch.aspx, and http://propaccess.traviscad.org/clientdb/PropertySearch.aspx?cid=1
    - [ ] This data is ready for incorporation into an experimental database.
    - [ ] Services have been prepared to regularly update this data source into database.
3. new building construction permits (street address resolution)
    * This factor consists of permits for new building construction in Austin Texas.
    - [x] The data source that provides up-to-date localized data has been identified.
        * This data originates from csv file available on this website: https://data.austintexas.gov/Building-and-Development/Issued-Construction-Permits/3syk-w9eu
    - [x] This data is ready for incorporation into an experimental database.
    - [ ] Services have been prepared to regularly update this data source into database.
                        +
4.-8. eviction rates from 2000-2016 (block group resolution) AND poverty rates from 2000-2016 (block group resolution).
AND median property value from 2000-2016 (block group resolution).
AND percent renter occupied from 2000-2016 (block group resolution).
AND population size from 2000-2016 (block group resolution).
    * The above factors consists of historical data for Travis County from 2000 to 2016 on: rates of actual eviction in each block group, rates of poverty in each block group, median property values of real property in each block group, percentage of residents in block group that are renters, and the size of population within a block group. 
    - [x] The data source that provides up-to-date localized data has been identified.
        * This data originates from csv file available on this website: https://eviction-lab-data-downloads.s3.amazonaws.com/TX/block-groups.csv
        * The relevant block groups can be restricted to those in Travis County.
    - [x] This data is ready for incorporation into an experimental database.
    - [ ] Services have been prepared to regularly update this data source into database.