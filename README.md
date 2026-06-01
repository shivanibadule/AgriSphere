#  AgriSphere - Smart Farming Platform

AgriSphere is an AI-powered agricultural companion designed to help farmers maximize profitability, detect crop diseases early, and access government benefits. This project was developed as a comprehensive solution for modern farming challenges.

## Key Features

*   ** AI Disease Detection:** Upload an image of an infected crop to get an instant diagnosis and expert treatment plan (Powered by Gemini 1.5 Flash).
*   ** Crop Profitability Advisor:** Automatically detects location to fetch real-time weather and soil data, recommending the most profitable crops.
*   ** Mixed Cropping Guide:** Smart suggestions for companion planting to improve yield and soil health.
*   ** Government Schemes:** Instant access to relevant Indian agricultural schemes and subsidies based on state.
*   ** Multi-Agent AI:** Uses **CrewAI** to coordinate specialized AI "agents" that act as virtual agricultural consultants.

##  Tech Stack

*   **Frontend:** Streamlit
*   **AI Models:** Google Gemini 1.5 Flash
*   **Orchestration:** CrewAI (Multi-agent framework)
*   **Data Sources:** OpenWeatherMap API, SoilGrids, Nominatim (OSM)

##  How to Run Locally

### 1. Download the Project
Download the source code as a ZIP file from this repository and extract it.

### 2. Install Python
Ensure you have Python 3.9 or higher installed on your system.

### 3. Install Required Libraries
Open your terminal/command prompt in the project folder and run:
```bash
pip install -r requirements.txt
```

### 4. Setup Environment Variables
Create a file named `.env` in the root folder and add your API keys:
```env
GEMINI_API_KEY=your_gemini_api_key
OPENWEATHER_API_KEY=your_openweathermap_key
GOOGLE_API_KEY=your_google_ai_studio_api_key
```

### 5. Start the App
Run the following command to launch the dashboard:
```bash
streamlit run streamlit_pages.py
```

## Project Structure
- `streamlit_pages.py`: The main dashboard and navigation hub.
- `image_detect.py`: AI logic for disease identification.
- `crop_adviser.py`: Soil and weather-based profitability analysis.
- `govt.py`: Government schemes database and search logic.
- `mycrew.py` & `config/`: AI Agent configurations for deep analysis.

---
**Note:** This project was built for the YCCE Hackathon.
