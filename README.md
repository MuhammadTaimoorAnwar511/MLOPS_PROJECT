# **Crypto-Price-Prediction-Website**  

This project is a complete MLOps implementation for a cryptocurrency price prediction system, focusing on Bitcoin. It includes backend data processing and model training, a React-based frontend, and deployment via Docker and Kubernetes.  

---

## **Team Members**
1. Taimoor Anwar (i21-1232)  
2. Ushna Nadeem (i21-1225)  
3. Fahad Bajwa (i20-2349)  

---

## **Overview**
The Crypto-Price-Prediction-Website fetches live cryptocurrency data, processes and cleans it, trains an LSTM model for price prediction, and visualizes live price charts using an interactive web application. The project utilizes modern MLOps tools and techniques to ensure automation, scalability, and version control.

---

## **Backend**
### **1. Fetch Live Data**
- Live cryptocurrency data for Bitcoin (1-day time interval) fetched from OKX.  
- Historical data for the past six months retrieved and stored in the `Data` folder.  

### **2. Cleaned Data**
- Raw data was cleaned and processed.  
- Cleaned data stored in the `Data` folder for subsequent usage.  

### **3. Model Training**
- Trained an **LSTM model** on the cleaned data.  
- Saved the trained model in `.h5` and `.pkl` formats for usage and backup.  

### **4. Model Versioning**
- Implemented model versioning using **MLflow UI**, enabling tracking and managing multiple model versions.  

### **5. Postman API Testing**
- APIs were tested using Postman for functionality verification.

---

## **Automation and Data Management**
### **1. Airflow**
- Installed and used **Apache Airflow** to automate the data fetching, cleaning, and training processes using Directed Acyclic Graphs (DAGs).  

### **2. Data Version Control (DVC)**
- **DVC** and **Google Cloud Storage** were employed for data versioning and storage management.

---

## **Frontend**
### **1. Development**
- Developed using **React**.  
- **MongoDB Atlas** used for database management.  
- Integrated **TradingView widget** for live price charts.  

### **2. Pages**
1. **Login Page**  
2. **Signup Page**  
3. **Prediction Page**  
4. **Live Chart Page**  

---

## **Containerization and Deployment**
### **1. Dockerization**
- Created Dockerfiles for both the frontend and backend.  
- Utilized **Docker Compose** for seamless containerization.  

### **2. Kubernetes Deployment**
- Deployed the application on **Kubernetes** using **Minikube**.  
- Uploaded container images to **Docker Hub**.  
- Deployment and service YAML files created for backend and frontend.  

---

## **Project Workflow**
### **1. GitHub Workflows**
- Implemented workflows to trigger actions based on branch changes, ensuring **Continuous Integration and Continuous Deployment (CI/CD)**.  

### **2. Git Repository**
- Maintained the project codebase in a Git repository for version control.  

---

## **Technologies Used**
- **Languages/Frameworks:** Python, React  
- **Database:** MongoDB Atlas  
- **MLOps Tools:** Airflow, MLflow, DVC, Google Cloud Storage  
- **Containerization and Orchestration:** Docker, Kubernetes (Minikube)  
- **APIs:** Postman Testing  
- **Version Control:** Git, GitHub  

---

## **How to Run**
### **1. Prerequisites**
- Docker and Docker Compose installed.  
- Kubernetes and Minikube configured.  
- MongoDB Atlas set up.  

### **2. Steps to Run**
#### **Backend**
1. Navigate to the backend directory:
   ```bash
   cd Backend
   ```
2. Install dependencies and run the backend:
   ```bash
   pip install -r requirements.txt
   python app.py
   ```

#### **Frontend**
1. Navigate to the frontend directory:
   ```bash
   cd Frontend
   ```
2. Install dependencies and start the frontend:
   ```bash
   npm install
   npm start
   ```

#### **Docker Compose**
To run the application using Docker Compose:
```bash
docker-compose up
```

#### **Kubernetes Deployment**
To deploy the application using Minikube:
```bash
kubectl apply -f Frontend-Deployment.yaml
kubectl apply -f Backend-Deployment.yaml
kubectl apply -f Frontend-Service.yaml
kubectl apply -f Backend-Service.yaml
```

---

## **Screenshots**
Include images of:
- MLflow UI
- Airflow DAGs
- Minikube Dashboard
- Application UI Pages (Login, Signup, Prediction, Live Chart)

---

## **Future Enhancements**
- Adding more cryptocurrencies for predictions.  
- Expanding the database for larger historical datasets.  
- Implementing additional machine learning models for better accuracy.  
- Enhancing frontend with advanced visualizations and dashboards.  

---

### **Contact**
For queries, reach out to the project contributors.  
