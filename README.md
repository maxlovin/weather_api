# 🌧️ Rain Alert SMS Notification

Automated Python script that checks the weather forecast for the next 12 hours using the OpenWeatherMap API and sends an SMS notification via Twilio if rain or snow is expected.

---

## 📌 Features

* Fetches 3-hour forecast data for the next 12 hours (`cnt=4`).
* Evaluates weather condition codes (IDs under 700 signify rain, drizzle, or snow).
* Automatically triggers an SMS alert to your phone via Twilio when precipitation is detected.

---

## 🛠️ Prerequisites & Setup

### 1. Requirements
* Python 3.x installed.
* An active **OpenWeatherMap** account and API key.
* An active **Twilio** account with a virtual phone number, Account SID, and Auth Token.

### 2. Installation

Clone the repository and install the required dependencies:

```bash
git clone [https://github.com/your-username/rain-alert-sms.git](https://github.com/your-username/rain-alert-sms.git)
cd rain-alert-sms
pip install requests twilio

```

---

## 🚀 Configuration & Usage

1. Open `main.py` (or your Python script file).
2. Update the configuration placeholders with your credentials:

```python
api_key = "YOUR_OPENWEATHERMAP_API_KEY"
account_sid = "YOUR_TWILIO_ACCOUNT_SID"
auth_token = "YOUR_TWILIO_AUTH_TOKEN"

# Set your target location coordinates
MY_LAT = 51.507351   # Example: London Latitude
MY_LONG = -0.127758  # Example: London Longitude

# Update Twilio phone numbers
from_ = "YOUR_TWILIO_VIRTUAL_NUMBER" # e.g., "+1234567890"
to = "YOUR_VERIFIED_PHONE_NUMBER"   # e.g., "+0987654321"

```

3. Run the script:

```bash
python main.py


```

```
