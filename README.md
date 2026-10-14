# SustainaRide
* This project is made by team CodeBritannic for the Uber Global Hackathon
* Top 6 teams in Europe and Central Asia
* [Watch the SustainaRide Video on YouTube](https://www.youtube.com/watch?v=9IeYVpJtRzQ)

## Key Features

*   **Interactive Map Interface**: Visualize your journey using a map powered by `TkinterMapView`. Users can search for addresses, set start and end points, and see the route drawn on the map.
*   **Intelligent Route Planning**: Utilizes `openrouteservice` to calculate and display the optimal path between two locations, providing distance information.
*   **AI-Powered Recommendations**: Employs OpenAI's GPT-3.5 Turbo to provide tailored travel advice. Based on your start and end points, the AI suggests the ideal mode of transport, comparing options like public transit and carpooling with estimated costs.
*   **Real-time Carpooling**:
    *   **For Drivers**: Drivers can register their details, specify a pickup radius in miles, and view a list of potential passengers in their vicinity. They receive requests from passengers and can choose to accept them.
    *   **For Passengers**: Passengers can find nearby drivers heading in their direction. They can send a request to a driver of their choice and receive a notification upon acceptance.
*   **Voice Interaction**:
    *   **Speech-to-Text**: Ask the AI assistant for travel advice using your voice. The application uses `AssemblyAI` to transcribe your speech into text.
    *   **Text-to-Speech**: Listen to the AI's recommendations read aloud, powered by `gTTS`.
*   **Customizable UI**: The application is built with `customtkinter`, offering a modern user interface with support for light and dark themes.

## Technologies Used

*   **GUI**: `customtkinter`, `tkintermapview`
*   **Mapping & Geocoding**: `openrouteservice-py`, `geopy`, `polyline`
*   **AI & Machine Learning**: `openai` (GPT-3.5-Turbo for recommendations), `AssemblyAI` (Speech-to-Text)
*   **Audio**: `gTTS` (Text-to-Speech), `pygame` (Audio playback), `pvrecorder` (Audio recording)
*   **Backend Communication**: `requests` (To interact with the PythonAnywhere-hosted server for carpooling)

### Prerequisites

You will need API keys for the following services. Please set them as environment variables in your system:

*   `OPENROUTESERVICE_API_KEY`
*   `OPEN_AI_API_KEY`
*   `ASSEMBLYAI_API_TOKEN`

### Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/suvir-dev/SustainaRide.git
    cd SustainaRide
    ```

2.  **Install the required Python packages:**
    ```sh
    pip install customtkinter tkintermapview openrouteservice geopy openai requests gTTS pygame pvrecorder assemblyai polyline certifi
    ```

### Running the Application

Once the dependencies are installed and environment variables are set, run the main application file:

```sh
python main.py

