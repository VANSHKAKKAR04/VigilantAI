# VigilantAI

AI-powered public safety and emergency response platform for detecting suspicious activity, reporting incidents, guiding safer routes, and connecting users with legal support when it matters most.

VigilantAI combines computer vision, real-time alerts, geospatial intelligence, and blockchain-backed evidence storage to help communities act faster and with more confidence in times of distress.

## Why this project matters

Safety systems are often fragmented: emergency reporting is slow, surveillance footage is hard to interpret, and critical evidence is vulnerable to tampering. VigilantAI aims to solve this by creating a unified platform that:

- detects crimes or suspicious activity from uploaded or live CCTV/video input
- surfaces real-time risk information on a city-level dashboard
- enables quick emergency reporting and SOS workflows
- suggests safer routes and nearby support services
- helps users access legal guidance and documentation support
- stores sensitive incident records in a more trustworthy and tamper-resistant way

## Core features

- AI crime detection using computer vision and video analysis
- Real-time alerts for emergency and high-risk scenarios
- Safer route suggestions based on crime hotspots and live data
- Complaint and FIR reporting with media uploads
- Legal assistance chatbot and rights guidance
- Emergency dashboard for monitoring incidents and alerts
- Decentralized reporting using blockchain smart contracts
- Wearable/health-device integration for broader safety monitoring

## Product vision

VigilantAI is designed to make safety more proactive, not reactive. Instead of waiting for incidents to escalate, the platform helps communities identify risk patterns earlier, respond faster, and document events more reliably.

The solution is especially useful for:

- public safety teams
- emergency response coordinators
- community organizations
- individuals seeking safer navigation and support
- legal aid and complaint-support workflows

## Tech stack

- Frontend: React + Vite + Tailwind CSS + Ant Design
- Backend API: Node.js + Express
- Database: MongoDB
- AI/ML inference: Python + Flask + PyTorch + OpenCV
- Blockchain: Ethereum smart contracts via Truffle
- Mapping and geo services: Leaflet / Map-based UI and geospatial data
- Web3 integration: Ethers / Web3.js

## Project structure

```text
VigilantAI/
├── client/                 # Frontend application
├── server/                 # Express backend for reports, emergency APIs, contact forms
├── models/                 # Python ML inference service for crime classification
├── blockchain/             # Solidity contracts and deployment configuration
├── wearable-device-backend/ # Fitbit / wearable integration backend
├── README.md               # Project overview and setup guide
└── backend/                # Additional backend or utility components
```

## How it works

1. A user records an incident, uploads media, or triggers an emergency alert.
2. The system captures location and contextual details.
3. The AI model analyzes uploaded or live video for suspicious patterns.
4. Alerts are pushed to relevant dashboards and response workflows.
5. Reports are saved and can be reviewed in the admin dashboard.
6. Legal guidance and safer route recommendations help users take immediate action.
7. Blockchain-based storage adds tamper resistance and trust to serious incident records.

## Features by module

### 1) Safety dashboard

The client app includes an interface for live monitoring, incident reporting, complaint submission, and hotspot visualization.

### 2) AI crime detection

The Python model in the `models/` folder classifies suspicious video activity and identifies patterns such as fighting, assault, or abnormal activity.

### 3) Report and emergency API

The `server/` application handles:

- complaint or FIR submission
- emergency SOS reporting
- media uploads
- contact messages
- dashboard data retrieval

### 4) Blockchain-backed evidence

The `blockchain/` folder contains the smart contract layer for secure, decentralized incident record management.

### 5) Wearable integration

The wearable backend supports health and device-based data integration to enrich safety workflows and emergency detection.

## Getting started

### Prerequisites

- Node.js 18+
- npm
- Python 3.9+
- MongoDB instance or local MongoDB service
- Ethereum dev environment (for blockchain features)

### 1. Clone the repository

```bash
git clone https://github.com/your-username/VigilantAI.git
cd VigilantAI
```

### 2. Frontend setup

```bash
cd client
npm install
npm run dev
```

The frontend typically runs on:

```text
http://localhost:5173
```

### 3. Backend setup

```bash
cd server
npm install
node server.js
```

The backend API will run on:

```text
http://localhost:5000
```

### 4. AI model setup

Use a Python environment and install the required libraries for computer vision and machine learning. Dependencies typically include:

- Flask
- PyTorch
- OpenCV
- torchvision
- Pillow

Then run the model service:

```bash
cd models
python app.py
```

### 5. Blockchain setup

```bash
cd blockchain
npm install
truffle develop
```

Then deploy the smart contracts as needed for the project workflow.

## Environment variables

For full functionality, configure environment variables for:

- MongoDB connection URI
- app secrets for the backend
- map or location service access
- wearable API configuration
- blockchain network settings

Create `.env` files in the relevant service folders as needed.

## Use cases

- rapid crime reporting from mobile or web applications
- CCTV-based suspicious activity classification
- emergency response coordination
- legal assistance for incident documentation
- safer route guidance in high-risk areas
- better evidence collection with tamper-resistant records

## Roadmap

- improve AI classification accuracy with larger datasets
- strengthen real-time alert orchestration
- add authenticated admin and response-team workflows
- expand geo-intelligence and route optimization
- improve privacy and security for sensitive records
- integrate more wearable and IoT safety signals

## Contributing

Contributions are welcome. To contribute:

1. fork the repository
2. create a feature branch
3. implement your changes
4. validate locally
5. submit a pull request with a clear summary

## License

This project is currently distributed under the repository's existing licensing terms. Please check the project files for the definitive license status before reuse or distribution.

## Acknowledgements

This project was built to demonstrate how AI, geospatial systems, and secure digital infrastructure can improve public safety and emergency response.
