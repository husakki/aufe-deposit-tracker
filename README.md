# AuFe deposit tracker
<sub>Au=Gold | Fe=Silver</sub>

An open-source tracker for precious metal deposits. It automates the tedious math of calculating silver and gold gains by comparing your historical purchase price against live market data. Monitor your "stack" value, track cost-averaging, and visualize your total ROI[^1] through a clean, intuitive dashboard.

## Features
- **Multi-Asset Management**
    - **Detailed Inventory:** Track gold and silver holdings with precision, including purchase price, weight (oz/g).
    - **Multiple Deposits:** Organize your holdings across different vaults.
- **Live Spot Prices**
    - Automatically fetches the most recent market data for gold and silver to ensure your portfolio value is always current.
    - Currency Support: *USD*, *EUR*, *GBP*
- **Financial Analytics & ROI[^1]**
    - **Profit/Loss Tracking:** Instantly see the difference between your acquisition cost and current market value.
    - **Revenue Visualization:** Monitor the total gross value of your deposits at a glance.
    - **Cost Basis Analysis:** Automatically calculates your *break-even* point for each asset.


## Installation
Make sure to have docker installed.  
Then just do `docker compose up -d` inside the root folder.

## Usage
Under `http://localhost:8080` the website for the application can be used.

## Techstack
**Database:** PostgreSQL  
**Backend:** Python 3.12 with [*fastapi*][1]  
**Frontend:** Flutter

> Flutter might be replaced with [*streamlit*][3]  
> [*scrapy*][2] might be used to get the live spot prices 

## Disclaimer & License
***Disclaimer:*** *This software is for tracking purposes only and does not constitute financial advice.*  

This project is licensed under the **GNU GENERAL PUBLIC LICENSE Version 3**.   
See the [LICENSE](LICENSE) file for the full text.

[^1]: ROI = Return of investment

[1]: https://fastapi.tiangolo.com/
[2]: https://www.scrapy.org/
[3]: https://streamlit.io/