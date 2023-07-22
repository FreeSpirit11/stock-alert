# Stock-Alert

Stock-Alert is a Python script that uses the Alpha Vantage API and News API to monitor stock prices and send SMS alerts if there is a significant change in the stock price of Tesla Inc (TSLA) along with related news headlines.

## Prerequisites

Before running the script, ensure you have the following:

1. Python 3 installed on your system.
2. Required Python packages: `requests`, `datetime`, and `twilio`.

```bash
pip install requests
pip install twilio
```

3. Create an account on [Twilio](https://www.twilio.com/) and get your Account SID and Auth Token.

## How to Use

1. Replace the placeholders in the script with your API keys and personal phone numbers.

```python
# Replace these placeholders with your actual API keys and phone numbers
account_sid = 'YOUR_ACCOUNT_SID'
auth_token = 'YOUR_AUTH_TOKEN'
STOCK = "TSLA" # YOUR STOCK SYMBOL HERE
COMPANY_NAME = "Tesla Inc" # YOUR COMPANY NAME
STOCK_API_KEY = "YOUR_STOCK_API_KEY"
NEWS_API_KEY = "YOUR_NEWS_API_KEY"
my_phone_number_twilio = "YOUR_TWILIO_PHONE_NUMBER"
my_real_phone = "YOUR_REAL_PHONE"
```

2. Run the script, and it will check for the percentage change in the stock price of Tesla Inc (TSLA) for the previous day. If the change is more than 10%, it will fetch related news headlines using the News API and send an SMS alert using Twilio.

```bash
python stock_alert.py
```

3. Sit back and relax! You will receive an SMS alert if there is a significant change in the stock price of Tesla Inc (TSLA) with related news headlines.

## Acknowledgement

This project was created as part of a #100daysofcode challenege by angela yu on udemy.Special thanks to the Alpha Vantage API and News API for providing free access to financial market data and news headlines.

## Author

[Mansi Yadav](https://github.com/FreeSpirit11)
