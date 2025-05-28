# Deployment Guide

_How to deploy seasonal pricing zones using Oracle Simphony Cloud's EMC_

## Steps

1. Prepare price level configuration
2. Log in to EMC and navigate to the appropriate hierarchy level([100000] - 'SA Master'; Sub Zone = [1] - 'SA Menu').
3. Zone Configuration "Add seasonal zones within the 'SA Master' zone {'Easter', 'Winter', 'Spring', 'Festive & B2W'}.
4. From the highest hierarchy level, add the following 'Effective Groups' {[1]; 'Easter Price Increase', [2]; 'Winter Price Increase', [3]; 'Spring Price Increase',[4]; 'Festive Price Increase'}
5. Set overrides to other 'Effective Groups' to expire from each Seasonal Zone, and leave only one active per identified Seasonal Zone.
6. In the identified seasonal zone 'Menu Item Maintenance', highlight all in 'Definition Records' but 'Header Records' override records with 'Keep Existing Record' as method
7. From the highest hierarchy level, 'Menu Item Maintenance', highlight all in 'Price Records' but 'Header Records', distribute records to each Seasonal Zone, and update 'Effective Groups' per identified Seasonal Zone.
8. All the 'Definition Records', 'Price Records' will be removed from the enterprise level, and master records will remain. 
