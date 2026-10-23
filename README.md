# Full-stack Developer Capstone - Cars Dealership Application

## Project Overview
This repository contains the Full-stack Development Capstone Project for **Cars Dealership**, a national car retailer in the United States. The web application allows visitors to view dealership branches across all 50 states, filter dealers by location, view existing customer reviews with automated sentiment analysis, and post new reviews for purchased vehicles.

## Architecture & Technology Stack
- **Frontend**: Dynamic UI built with React.js, HTML5, CSS3, and Bootstrap for responsive design.
- **Backend (User Management & Inventory)**: Python and Django REST framework for user authentication, registration, car makes, and car model inventory management.
- **Microservices (Dealerships & Reviews)**: Node.js and Express running on MongoDB to manage dealership records and customer feedback.
- **Sentiment Analysis**: Python and Flask microservice using NLTK (VADER SentimentIntensityAnalyzer) to classify customer review sentiment as positive, neutral, or negative.
- **CI/CD & DevOps**: GitHub Actions for automated linting (flake8, jshint), Docker containerization, Kubernetes orchestration, and IBM Cloud Code Engine deployment.

## Repository Structure
- `server/djangoproj`: Core Django project configuration and routing.
- `server/djangoapp`: Django application containing models, views, templates, and REST API adapters.
- `server/djangoapp/microservices`: Flask microservice for NLTK sentiment analysis.
- `server/database`: Express and MongoDB service with Mongoose models and dataset seed files.
- `server/frontend`: React frontend application and static pages (About Us, Contact Us).
- `.github/workflows`: Continuous Integration (CI) workflow configuration.

## Features
1. **Dealer Management**: Interactive table listing dealerships with state filtering.
2. **Review System**: Detailed reviews per dealer with visual sentiment classification emojis/badges.
3. **User Authentication**: Secure user registration, login, and logout.
4. **Car Inventory**: Database records connecting Car Makes and Car Models with inline Django admin controls.
5. **Post Reviews**: Form for verified car buyers to submit dealer ratings and review feedback.