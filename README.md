# Slack AI Community Lead Qualifier

This project is an intelligent AI-powered Slack bot that automatically researches new community members as they join, scores their potential as a customer, and reports the findings to a private channel. Built with Node.js, OpenAI, LangChain, and PostgreSQL, this tool helps community managers and SaaS founders qualify leads in real time.

## 🚀 Features

**Automated Lead Research**  
Detects new member joins through the Slack Events API.

**AI Analysis**  
Uses OpenAI and LangChain to research members via GitHub and web lookups, then calculates a fit score based on company and product criteria.

**Data Persistence**  
Automatically saves lead profiles and analysis results to a PostgreSQL database hosted on Render.

**Private Notifications**  
Delivers formatted reports directly to a private Slack channel using Block Kit.

## 🛠 Tech Stack

- **Backend:** Node.js, Express
- **AI Framework:** LangChain and OpenAI
- **Database:** PostgreSQL with the `pg` library
- **Communication:** Slack Bolt API
- **Deployment:** Render with Blueprint support

## 📋 Setup and Installation

### 1. Clone the repository

    git clone https://github.com/ameyg11/slack-ai-agent.git
    cd slack-ai-agent

### 2. Install dependencies

    npm install

### 3. Configure environment variables

Create a `.env` file in the root directory and add the following:

    SLACK_BOT_TOKEN=xoxb-...
    SLACK_APP_TOKEN=xapp-...
    SLACK_SIGNING_SECRET=...
    SLACK_PRIVATE_CHANNEL_ID=...
    OPENAI_API_KEY=sk-...
    DATABASE_URL=postgres://...
    COMPANY_NAME=Your Company Name
    COMPANY_PRODUCT=Your Product Name
    NODE_ENV=development

### 4. Run the application

    npm start

## ☁️ Deployment

This project is designed to be deployed on Render using the included `render.yaml` blueprint. Connect your GitHub repository to Render to automate the build and deployment process.

## 💡 Acknowledgements

This project was developed based on the Build Your Own AI Agent course by Ania Kubow, supported by Render and freeCodeCamp.
