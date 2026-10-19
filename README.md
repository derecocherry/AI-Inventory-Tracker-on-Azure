# AI-Inventory-Tracker-on-Azure
An event-driven inventory system. Sale events are buffered in Azure Service Bus and processed by an Azure Function that updates stock counts in Azure SQL in near real time. Each morning, a Logic App summarizes 30 days of sales, asks Azure OpenAI for restock recommendations, and emails the result. Infrastructure is provisioned with Terraform.
