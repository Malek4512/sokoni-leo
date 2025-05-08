Project Plan: Local Market Price Tracker
1. Project Overview

Name: Local Market Price Tracker
Objective: Develop a system that tracks and displays real-time or regularly updated market prices for key commodities (e.g., maize, rice, sugar, fish) across different regions.
Target Users: Farmers, traders, market analysts, and the general public.
Key Channels: SMS, WhatsApp bot, and Web application.
Data Source: Crowdsourced and verified user submissions.
2. Key Features

    Regional price listings for commodities.

    Crowd submission of prices with verification.

    Admin panel for managing submissions.

    SMS interface for offline users.

    WhatsApp bot for chatbot interaction.

    Web app with a dashboard and analytics.

3. Timeline (Gantt-style Milestones)
Phase	Description	Duration
Requirement Analysis	Define features, roles, and data flow	1 week
Design	UI/UX for web, chatbot flows, SMS command structure	1 week
Backend Development	API, database, admin panel	2 weeks
Frontend & Bot Dev	Web app, WhatsApp integration	2 weeks
SMS Integration	Integrate SMS gateway and keyword logic	1 week
Testing & QA	Validate all flows and data accuracy	1 week
Deployment & Feedback	Go live + pilot testing in one region	1 week
Expansion	Roll out to more regions + optimize	Ongoing
4. Tools & Technologies

    Frontend: React / HTML-CSS / Bootstrap

    Backend: Node.js or Django / Flask

    Database: PostgreSQL or MongoDB

    Bot: Twilio WhatsApp API / Dialogflow

    SMS: Africa’s Talking / Twilio SMS API

    Hosting: AWS / DigitalOcean / Heroku

📄 Software Requirements Specification (SRS)
1. Introduction
1.1 Purpose

To design and implement a system that enables users to view, submit, and retrieve market prices of key agricultural and consumer goods across different regions.
1.2 Scope

The system supports:

    Display of commodity prices by region

    Crowdsourced data submissions

    Multi-platform access (SMS, WhatsApp, Web)

    Role-based access for admins and users

1.3 Definitions

    Commodity: Item being priced (e.g., maize)

    Crowdsourced Data: User-submitted price information

    Verified Price: Admin-approved or majority-voted data

2. System Features
2.1 View Prices

    View latest commodity prices by selecting region and item.

    Filter by date, location, and commodity type.

2.2 Submit Price

    Users can submit price data for a specific commodity and region.

    Include optional photo evidence or market name.

2.3 Admin Panel

    View and approve submitted prices.

    Manage users and moderate submissions.

2.4 SMS Interface

    Users send SMS in format:
    PRICE <commodity> <price> <region>
    or request: GET <commodity> <region>

2.5 WhatsApp Bot

    Respond to keyword inputs like:

        “Prices in Dodoma”

        “Submit maize 1200 Morogoro”

2.6 Web Dashboard

    Interactive UI to view prices on charts, maps.

    Data export and statistics for admins.

3. Non-Functional Requirements

    Scalability: Capable of handling thousands of users daily.

    Reliability: System should have >99% uptime.

    Security: Authenticated admin access, data validation.

    Performance: Query response in under 2 seconds.

    Usability: Simple interfaces for low-tech users.

4. System Architecture

    3-tier Architecture:

        Presentation (Web, Bot, SMS)

        Logic (APIs)

        Data (Database)

5. Constraints

    Limited or unreliable internet access in rural areas.

    SMS and WhatsApp cost handling.

    Language localization (e.g., Swahili)

6. Assumptions

    Users have basic literacy or access to mobile phones.

    Admins available to validate price data.

    Pricing updates are frequent but not necessarily real-time.
