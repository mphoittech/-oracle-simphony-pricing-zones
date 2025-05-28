# Deployment Guide

_How to deploy seasonal pricing zones using Oracle Simphony Cloud's EMC_

## Steps

1. Prepare price level configuration
2. Log in to EMC and navigate to the appropriate hierarchy level([100000] - 'SA Master'; Sub Zone = [1] - 'SA Menu').
3. Zone Configuration "Add Seasonal Zones within the 'SA Master' Zone {'Easter', 'Winter', 'Spring', 'Festive & B2W'}.
4. From the highest hierarchy level, add the following 'Effective Groups' {[1]; 'Easter Price Increase', [2]; 'Winter Price Increase', [3]; 'Spring Price Increase',[4]; 'Festive Price Increase'}
5. In each Seasonal Zone's 'Menu Item Maintenance', highlight all in 'Definition Records' but 'Header Records' override records with 'Keep Existing Record' as method
6. From the highest hierarchy level, 'Menu Item Maintenance', highlight all in 'Price Records' but 'Header Records', distribute records to each Seasonal Zone, and validate price records.
7. Deploy the properties to selected zones/outlets, keeping per (Halaal / non-Halaal).
8. Confirm deployment via system logs and spot checks.
