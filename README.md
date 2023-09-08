# Introduction 
This componet is for use on partner websites to display match odds for various leagues.
The matches and leagues are managed by Eyas as a "coupon".  
The component will contain the coupon ID.  
There are two coupon IDs, one for prod and one for non prod (testing)
There are 3 test pages here, one for the Production component, one for Eyas UAT coponent, and one for  Eyas DEV component (only visible to eyas)
The component will show a horizontal "swim lane" of match cards per league.

# Getting Started
Add the following HTML to the page:

<eyas-fixture-swimlanes coupon-id="35" max-events-displayed="20" ></eyas-fixture-swimlanes>


## parameters:
 - coupon-id this will be supplied by Eyas, and contains a curated list of events and leagues.
 - max-events-displayed this will limit the width of each leages "swim lane".


# support
For technical support, please email simon hobbs @ eyasgaming or use the teams channel