# Introduction 
This componet is for use on partner websites to display match odds for various leagues.
The matches and leagues are managed by Eyas as a "coupon".  
The component will contain the coupon ID.  
There are two coupon IDs, one for prod and one for non prod (testing)
There are 3 test pages here, one for the Production component, one for Eyas UAT coponent, and one for  Eyas DEV component (only visible to eyas)
The component will show a horizontal "swim lane" of match cards per league.

# Getting Started
Add the following HTML to the page:

```
    <head>
        <!-- ONLY INCLUDE SCRIPT ONCE PER PAGE -->
        <script src="https://lancebetting.com/etc.clientlibs/eyas-web/clientlibs/external-components.latest.js" data-eyas-config="https://lancebetting.com/content/eyas-web/lancebet_com/pt.client.settings.json" async></script>
    </head>

    <body>

        <eyas-fixture-swimlanes coupon-id="35" max-events-displayed="20" ></eyas-fixture-swimlanes>
```

See index.html for example code. 

see https://brave-coast-06ff01503.3.azurestaticapps.net/index.html for working site.


## parameters:
 - **coupon-id** this will be supplied by Eyas, and contains a curated list of events and leagues.
 - **max-events-displayed** this will limit the width of each leages "swim lane".

# environments
There are 3 environments which can have different versions of the component, dev, uat and prod.
Dev is hidden behind the VPN, but UAT and prod can be used.

to switch between environment, change the URL in the script and config section, e.g.

```
Prod:
        <script src="https://lancebetting.com/etc.clientlibs/eyas-web/clientlibs/external-components.latest.js" data-eyas-config="https://lancebetting.com/content/eyas-web/lancebet_com/pt.client.settings.json" async></script>
 UAT:       
        
          <script src="https://lancebet-com-uat.eyasgaming.net/etc.clientlibs/eyas-web/clientlibs/external-components.latest.js" data-eyas-config="https://lancebet-com-uat.eyasgaming.net/content/eyas-web/lancebet_com/pt.client.settings.json" async></script>
        
```


# support
For technical support, please email simon hobbs @ eyasgaming or use the teams channel