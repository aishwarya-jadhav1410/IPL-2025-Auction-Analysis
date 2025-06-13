# IPL-2025-Auction-Analys
📌 Overview
This Power BI dashboard provides insights into the IPL 2025 auction—covering player sales, team spending, and country-wise player stats.

✅ Key Features
Top Sold Players

Indian vs Overseas Player Breakdown

Team-wise Auction Spending

Country-wise Player Count

Filters by Team, Country, Player Type

⚙️ Main DAX Measures
DAX
Copy
Edit
Player Type = IF('Sold_Player'[Country] = "India", "Indian", "Overseas")

Top Sold Player = 
VAR TopPlayer = TOPN(1, ALL('Sold_Player'), 'Sold_Player'[Amount], DESC)
RETURN MAXX(TopPlayer, 'Sold_Player'[Player Name])
💻 Tools Used
Power BI Desktop

DAX

Power Query

👩‍💻 Created By
Aishwarya Jadhav | Data Analyst

Let me know if you want this in a PDF or .md file format.








