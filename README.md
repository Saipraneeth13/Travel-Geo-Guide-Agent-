# Multi-Agent Travel Itinerary Planner

Welcome to the **AI Travel Itinerary Planner**, a modular multi-agent application built using Streamlit, LangGraph, LangChain, and Ollama. The system leverages multiple AI agents to generate personalized travel itineraries and provide intelligent travel recommendations based on user preferences.

- **Repository:** https://github.com/vikrambhat2/MultiAgents-with-Langgraph-TravelItineraryPlanner

---

## Overview

The AI Travel Itinerary Planner uses a LangGraph-based workflow to coordinate multiple specialized AI agents that collaboratively generate a complete travel experience. Based on user inputs such as destination, duration, and travel month, the system creates personalized itineraries, activity recommendations, weather forecasts, packing suggestions, food and culture insights, and travel resources.

The project integrates:
- **Ollama** with the `llama3.2` model for local LLM inference
- **Google Serper API** for web search capabilities
- **Streamlit** for an interactive user interface
- **LangGraph** for orchestrating multi-agent workflows

---

## Features

- Personalized day-wise travel itinerary generation
- Smart local activity recommendations
- Real-time weather insights
- Packing list generation based on destination and season
- Food and cultural recommendations
- Useful travel resource links
- Conversational travel assistant for itinerary-related queries
- PDF export functionality for generated itineraries
- Modular multi-agent architecture for scalability and maintainability

---

## Project Structure

```bash
MultiAgents-with-Langgraph-TravelItineraryPlanner/
│
├── agents/
│   ├── generate_itinerary.py
│   ├── recommend_activities.py
│   ├── fetch_useful_links.py
│   ├── weather_forecaster.py
│   ├── packing_list_generator.py
│   ├── food_culture_recommender.py
│   └── chat_agent.py
│
├── export_utils.py
├── travel_agent.py
├── requirements.txt
└── .env
```

### Description

- **agents/** → Contains modular AI agents responsible for different travel-related tasks.
- **travel_agent.py** → Main Streamlit application and workflow controller.
- **export_utils.py** → Utility functions including PDF export support.
- **requirements.txt** → Project dependencies.
- **.env** → Environment variables and API keys.

---

## Installation

### Prerequisites

- Python 3.8+
- Ollama installed locally
- `llama3.2` model downloaded
- Google Serper API Key

### Clone the Repository

```bash
git clone https://github.com/vikrambhat2/MultiAgents-with-Langgraph-TravelItineraryPlanner.git

cd MultiAgents-with-Langgraph-TravelItineraryPlanner
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file in the root directory:

```env
SERPER_API_KEY=your_api_key_here
```

### Start Ollama

```bash
ollama serve
```

Pull the required model:

```bash
ollama pull llama3.2
```

---

## Running the Application

Start the Streamlit application:

```bash
streamlit run travel_agent.py
```

Then open the local URL provided by Streamlit:

```bash
http://localhost:8501
```

---

## Usage

1. Enter travel details such as:
   - Destination
   - Travel month
   - Duration
   - Preferences

2. Generate a personalized itinerary.

3. Explore:
   - Weather forecasts
   - Packing suggestions
   - Food and culture insights
   - Recommended activities
   - Useful travel resources

4. Interact with the AI travel assistant for itinerary-related queries.

5. Export the generated itinerary as a PDF.

---

## Future Enhancements

- Integration with live flight and hotel APIs
- Budget estimation and trip cost analysis
- Multi-language support
- Interactive maps and route optimization
- Real-time travel alerts and recommendations

---

## Contributing

Contributions are welcome! Feel free to:
- Fork the repository
- Open issues
- Submit pull requests
- Improve agent workflows or UI components

---

## Tech Stack

- Python
- Streamlit
- LangGraph
- LangChain
- Ollama
- Google Serper API

---

## License

This project is open-source and available under the MIT License.

---

## Contact

For queries or collaborations:

- **LinkedIn:** https://www.linkedin.com/in/vikrambhat249/
- Open an issue in the repository
