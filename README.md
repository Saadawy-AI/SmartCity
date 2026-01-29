🔷 Project Overview
Smart City Real-Time Data Engineering Platform.

🔷 Architecture Diagram
ERD Diagram.pdf 

🔷 Technologies
Python
Apache Kafka
Apache Spark Structured Streaming
Docker & Docker Compose

🔷 Data Flow
IoT Sensors → Kafka → Spark Streaming → AWS S3

🔷 How to Run
Bash
docker-compose up -d
python jops/main.py
spark-submit jops/spark-city.py
🔷 Folder Structure
SmartCity/
│
├── jops/
│   ├── config.py
│   ├── main.py
│   └── spark-city.py
│
├── ERD Diagram.pdf
│
├── docker-compose.yml
│
└── requirements.txt

🔷 Use Cases
Traffic monitoring
Pollution analysis
Emergency detection
Smart transportation
