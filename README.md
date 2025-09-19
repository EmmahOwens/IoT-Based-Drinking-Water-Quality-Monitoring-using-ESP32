# IoT-Based Drinking Water Quality Monitoring System

## Project Overview
This repository contains the initial setup for Assignment 1: Problem Identification and SDG Selection. The project focuses on addressing SDG 6 (Clean Water and Sanitation) by proposing a Wireless Sensor Network (WSN)/IoT solution for real-time monitoring of drinking water quality using ESP32 microcontrollers. Inspired by an open-source prototype, the system measures key parameters like electrical conductivity (EC) via Total Dissolved Solids (TDS) and temperature to detect contamination in remote or underserved areas.

## SDG Overview
The United Nations Sustainable Development Goals (SDGs) aim to tackle global challenges by 2030. SDG 6 targets "Clean Water and Sanitation," ensuring availability and sustainable management of water for all. Key targets include universal access to safe drinking water (6.1) and improved water quality by reducing pollution (6.3). As of 2025, approximately 2 billion people lack safely managed drinking water, heightening risks from waterborne diseases. This project leverages WSN/IoT to support these targets through real-time data collection.

## Problem Identification
### Scope
Contaminated drinking water causes significant health issues, with over 485,000 annual deaths from diarrheal diseases, mainly in low-income regions. In rural areas, sources like wells and reservoirs are vulnerable to pollutants from agriculture, industry, and natural sources, leading to high TDS levels exceeding WHO guidelines (e.g., EC > 400 μS/cm).

### Stakeholders
- **End-users**: Communities dependent on local water sources.
- **Governments and Regulators**: Water authorities monitoring SDG compliance.
- **International Organizations**: WHO and UN agencies providing guidelines.
- **Utilities and NGOs**: Managers of water distribution and sanitation.
- **Researchers/Developers**: Tech experts in IoT solutions.

### Current Gaps
Manual testing is infrequent, expensive, and lacks real-time capabilities, especially in remote areas. Gaps include absent continuous monitoring, infrastructure limitations, and poor data integration for global reporting.

## WSN/IoT Proposal
We propose a scalable WSN system using ESP32 for real-time water quality monitoring.

### System Architecture
- **Sensor Nodes**: ESP32 microcontroller with TDS sensor (0-1000 ppm) for EC, DS18B20 for temperature (-55°C to 125°C), and optional OLED display.
- **Networking**: WiFi or mesh (e.g., ESP-NOW) to relay data to a cloud platform like ThingSpeak.
- **Data Flow**:
  1. Sample data every 15 seconds.
  2. Process readings (e.g., temperature-compensated EC).
  3. Transmit via HTTP to cloud for storage, alerts (e.g., if EC > threshold), and dashboards.
- **Scalability**: Solar-powered nodes for 10-50 unit deployments in remote setups.

This solution enables early contamination detection, outperforming manual methods with automation and potential ML integration for predictions.

## Feasibility Check
### Constraints
- **Budget**: $50-100 per node (~$750 for 10-node pilot), affordable for academic use.
- **Hardware**: Readily available via online suppliers; open-source compatible.
- **Ethical/Technical**: Ensure data privacy (GDPR), community training; address battery life (solar) and sensor maintenance.

### Team Roles and Timeline
For a 4-member team (1-week deadline):
- **Member 1**: Research/SDG analysis (Days 1-2).
- **Member 2**: Hardware prototyping (Days 3-4).
- **Member 3**: Software/cloud integration (Days 3-4).
- **Member 4**: Report, presentation, and repo management (Ongoing).
- **Milestones**: Research (Days 1-2), Design (3-4), Drafting/Setup (5-6), Submission (7).

## Conclusion
This WSN/IoT solution aligns with SDG 6 by enabling proactive water quality management, bridging monitoring gaps in vulnerable regions. It promotes sustainable development through cost-effective tech, with potential for broader impacts via advanced analytics.
