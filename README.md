# civic-incident-data-platform
# Civic Incident Data Platform

This project was developed for BUS5001 – Cloud Platforms and Analytics.

## Overview
The solution uses Microsoft Azure to process local council incident data from CSV files and publish a public community dashboard.

## Azure Services
- Azure Blob Storage
- Azure Logic Apps
- Azure Static Website
- Managed Identity / RBAC

## Data Flow
1. CSV uploaded to the private `raw-data` container.
2. Azure Logic App validates and transforms the data.
3. Incident metrics and summaries are generated.
4. Public-safe JSON is created.
5. The Azure static website displays the dashboard.

## Dashboard
The dashboard displays:
- Total incidents
- Open incidents
- Resolved incidents
- In-progress incidents
- Incidents by category
- Incidents by priority
- Recent incident records

## Public Dashboard
https://stcouncilincidents260812.z8.web.core.windows.net/
