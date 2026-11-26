# Christian Trinidad
General Portfolio

# Project 1 : Windows Security Monitoring Lab 
•	Deployed a Windows VM in Microsoft Azure and configured a data collection rule by creating a Log analytics workspace and linking it to a SIEM (Sentinel), installing Windows Security Events, then installing Windows Security Events via AMA to send Windows seurity events through our Honeypot to a Log Analytics workspace linked to Microsoft Sentinel.

•	Reviewed Windows Security logs on our log analytics workspace and queried the SecurityEvent table using Kusto Query Language(KQL) to filter for the Administrator account and select relevant fields.
`
SecurityEvent
|where Account = "\\Administrator"
|project TimeGenreted, Account, Computer, EventID, Activity, IpAddress
`

•	Configured a Sentinel workbook using a GeoIP watchlist and provided a query to map failed sign-ins (Event ID 4625) by source IP location and show the number of attempts from each location.

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/0af3b3d5-10af-40a1-b135-0ca4aacb8758" />
