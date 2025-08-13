# OTX IPv4 General Threat Intelligence API

This project provides a custom ETL connector to interact with the **AlienVault OTX (Open Threat Exchange)** API to fetch threat intelligence details for a given IPv4 address.

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/otx_ipv4_general.git
cd otx_ipv4_general
```


### 2. Install Dependencies
```bash
pip install requests
```

### 3. Create and Activate Virtual Environment

CHECKKK
```bash
python -m venv venv
# On Windows
venv\Scripts\activate
# On Mac/Linux
source venv/bin/activate
```

### 4. Configure Environment Variables
Copy the template file and update it with your actual values:
```bash
cp ENV_TEMPLATE .env
```


### 5. Run the Connector

Run for a single IP:
```bash
python etl_connector.py 8.8.8.8
```

Run for multiple IPs:
```bash
python etl_connector.py 8.8.8.8 1.1.1.1
```
If no IP is provided, the script defaults to 8.8.8.8.

---

## API Endpoint Details
**Base URL:** `https://otx.alienvault.com/api/v1/indicators/IPv4/<IPv4_Address>/general`

Method:
GET

Headers:
json
{
  "X-OTX-API-KEY": "<Your_API_Key>",
  "Content-Type": "application/json"
}

---

## Example Output


### Logs

### MongoDB


## Author
**Name:** Niya  
**Role:** Developer  
**Contact:** [youremail@example.com]  

---

