# Ecotrack_repository
README-

EcoTrack

EcoTrack is a cloud-based web application designed to help users track and reduce their carbon footprint by monitoring energy consumption, transportation usage, and waste generation. The application provides insights, a user-friendly dashboard, and an interactive chatbot, "EcoBot," to guide users on sustainable practices.

Table of Contents

1. Project Overview


2. Features


3. Technologies Used


4. Setup and Installation


5. Usage


6. Architecture


7. License



Project Overview

EcoTrack empowers users to monitor and minimize their environmental footprint by providing actionable insights on carbon emissions. The project utilizes Vultr's cloud infrastructure to ensure scalability, security, and high performance, with backend services built in Flask and Laravel.

Features

User Registration & Login: Users can register and securely log in to access personalized insights.

Dashboard with Insights: A clean dashboard that displays summary insights on energy, transportation, and waste.

Visualized Emissions Overview: Interactive charts and graphs showing user-specific emissions data.

EcoBot (Chatbot): A chatbot powered by Llama 7B and integrated via Vultr’s serverless inference, providing advice on sustainable practices.

Data Entry Forms: Allows users to input their energy, transportation, and waste data for analysis.

Real-time Recommendations: Generates recommendations based on user inputs.


Technologies Used

Frontend: HTML, CSS, JavaScript, Chart.js

Backend: Flask (for main functionalities), Laravel (for chatbot integration)

Database: MySQL

Cloud Platform: Vultr (Ubuntu 1vCPU AMD, Mumbai server)

Chatbot Model: Llama 7B, integrated through Vultr’s serverless API


Setup and Installation

Prerequisites

Ensure you have the following installed:

Python 3.x

PHP 7.x or higher

Composer

Vultr API Key with permissions set up


Installation Steps

1. Clone the Repository:

git clone <repository-url>
cd EcoTrack


2. Set Up Flask Backend:

Navigate to the root directory and install dependencies:

pip install -r requirements.txt

Run the Flask application:

nohup python3 app.py &



3. Set Up Laravel for Chatbot:

Navigate to the chatbot directory and install dependencies:

composer install

Start the Laravel server:

php artisan serve --host=0.0.0.0 --port=8000



4. Environment Configuration:

Set your Vultr API key in the .env file for the chatbot.



5. Database Configuration:

Ensure MySQL is set up with tables for users and emissions:

Create tables using the schema provided in the /database/schema.sql file.



6. Run the Application:

Access Flask (dashboard and main functions) at http://<server-ip>:5000.

Access Laravel (chatbot) at http://<server-ip>:8000/chatbot.




Usage

1. Sign Up/Login: Register a new account or log in with existing credentials.


2. Dashboard Access: View summary insights and input your energy, transportation, and waste data.


3. Visual Data: Analyze your emissions data through charts and graphs on the dashboard.


4. Chat with EcoBot: Get sustainability tips by interacting with EcoBot in real-time.



Architecture

EcoTrack consists of a Flask and Laravel backend hosted on Vultr's cloud services. The dashboard aggregates user input for analysis and visualization, while EcoBot (hosted in Laravel) provides interactive guidance.

Key architecture components include:

1. Client/User Interface: User interaction layer for data input, chat, and visualization.


2. Backend: Flask handles dashboard and API requests; Laravel connects to Vultr’s API for the chatbot.


3. Database: MySQL stores user information and emissions data.


4. Vultr Cloud Services: Used for hosting and serverless inference.



License

EcoTrack is licensed under the MIT License. See the LICENSE file for more details.



