🌆 Smart City – Real-Time Data Engineering Platform

📌 Project Overview

Smart City is an end-to-end real-time data engineering platform designed to simulate and process smart city data such as traffic, GPS, weather, cameras, and emergency events.

The project demonstrates how modern cities can collect massive streaming data, process it in real time, and store it in a cloud-based data lake for analytics and AI applications.

This system is built using Apache Kafka, Apache Spark Structured Streaming, Docker.

---

🏗️ System Architecture

IoT Data Sources
(Vehicles, GPS, Cameras,
Weather, Emergency)
        ↓
Apache Kafka (Streaming)
        ↓
Apache Spark Structured Streaming


---

⚙️ Technologies Used

🔹 Programming

Python 3


🔹 Data Streaming

Apache Kafka

Apache Zookeeper


🔹 Data Processing

Apache Spark Structured Streaming


🔹 Containerization

Docker

Docker Compose



---

📂 Project Structure

SmartCity/
│
├── jops/
│   ├── config.py          # Configuration settings
│   ├── main.py            # Kafka producers & data simulation
│   └── spark-city.py      # Spark streaming processing job
│
├── ERD Diagram.pdf        # Database entity relationship diagram
│
├── docker-compose.yml     # Kafka, Zookeeper, Spark cluster
│
├── requirements.txt       # Python dependencies
│
└── README.md


---

🔄 Data Flow Explanation

1. Data Simulation

Smart city sensors are simulated using Python.

Data includes:

Vehicle information

GPS location data

Camera events

Weather data

Emergency alerts




2. Kafka Streaming

Each data source publishes messages to Kafka topics.

Zookeeper manages Kafka brokers.



3. Spark Structured Streaming

Spark consumes real-time data from Kafka.

Applies schemas and transformations.

Cleans and enriches incoming events.




---

🚀 How to Run the Project

1️⃣ Clone the Repository

git clone https://github.com/Saadawy-AI/SmartCity.git
cd SmartCity


---

2️⃣ Install Python Dependencies

pip install -r requirements.txt


---

3️⃣ Start Services Using Docker

docker-compose up -d

This will start:

Zookeeper

Kafka Brokers

Spark Master

Spark Workers



---

4️⃣ Run Kafka Producers

python jops/main.py

This will generate and stream smart city events into Kafka topics.


---

5️⃣ Run Spark Streaming Job

spark-submit jops/spark-city.py

Spark will:

Read data from Kafka

Process streaming events

Store results into AWS S3



---

📊 Use Cases

🚦 Traffic congestion monitoring

🛰️ Real-time vehicle tracking

🌦️ Weather impact analysis

🚨 Emergency event detection

🏙️ Smart transportation systems

---

🧠 Future Improvements

Real-time dashboard (Streamlit / Power BI)

Machine learning models:

Traffic prediction

Accident risk prediction

Energy consumption forecasting


Integration with AWS Athena

Real IoT sensor integration



---

👨‍💻 Author

Mohamed El-Sameen
Faculty of Computers & Artificial Intelligence
Minya National University

Data Engineering Enthusiast

Machine Learning (NTI)

Data Engineering (DEPI)
---

⭐ Final Notes

This project simulates an enterprise-level smart city data platform and reflects real-world data engineering architectures used in large-scale systems.

If you find this project useful, feel free to ⭐ the repository.


---

🚀 Built for learning, scalability, and real-time data engineering.
