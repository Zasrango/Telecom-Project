
# Telecom-Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/4e4ccb19-e449-4bb2-8ba8-de17d3f1c26b/ReportSection?experience=power-bi&clientSideAuth=0

## Problem Statement

Atliqo launched 5G plan on May 22 along with other telecom prviders. There is decline in revenue growth and decline in active users post period of 5G lauch.

This dashboard gives us comparasion between  pre lauch and post lauch of 5G

Metrics Used in this project :

1. Total Revenue = SUM(fact_atliqo_metrics[atliqo_revenue_crores]) 
2. AVG Revenue = AVERAGE(fact_atliqo_metrics[atliqo_revenue_crores])
3. AVG_RPU(Revenue Per User) = AVERAGE(fact_atliqo_metrics[arpu])
4. Total Active users = SUM(fact_atliqo_metrics[active_users_lakhs])
5. Total unsubscribed Users = SUM(fact_atliqo_metrics[unsubscribed_users_lakhs])
6. AVG Active Users = AVERAGE(fact_atliqo_metrics[active_users_lakhs])
7. AVG ms_pct = AVERAGE(fact_market_share[ms_pct])
8. AVG_REV_bfr 5G = CALCULATE([AVG Revenue],dim_date[before/after_5g]="Before 5G")
9. AVG_REV_afr 5G = CALCULATE([AVG Revenue],dim_date[before/after_5g]="After 5G")
10. ARPU_Bfr 5G = CALCULATE([AVG_RPU],dim_date[before/after_5g]="Before 5G")
11. ARPU_afr 5G = CALCULATE([AVG_RPU],dim_date[before/after_5g]="After 5G")
![Screenshot (15)](https://github.com/Zasrango/Telecom-Project/assets/169545862/479cc7f7-287a-4035-a15c-cd7a3f8df133)
