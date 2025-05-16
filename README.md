
<<<<<<< HEAD

Key Features
📦 Project Templating: Auto-generated structure using template.py

🐍 Python Virtual Environment: Easily setup with conda

🧪 Modular ML Pipeline: Clean separation of concerns — ingestion, transformation, training, evaluation

🌐 MongoDB Atlas Integration: Centralized and scalable NoSQL storage

🔒 Custom Logging & Exception Handling

📊 EDA & Feature Engineering: Notebook-ready analysis

📥 Data Ingestion via MongoDB ➜ Pandas

✅ Data Validation with Schema YAML

🔄 Data Transformation + Model Training

☁️ AWS S3 for Model Registry

🧠 Model Evaluation + Conditional Model Push

🧾 Prediction API with FastAPI/Flask

🐳 Dockerized App + .dockerignore

⚙️ CI/CD using GitHub Actions + AWS ECR + EC2

🔐 IAM Role Management for secure access


Project Workflow
✅ Phase 1: Project Setup
Set up modular Python structure with template.py.

Configure setup.py and pyproject.toml for package installation.

Create virtual environment: conda create -n vehicle python=3.10

Install all dependencies via requirements.txt.

✅ Phase 2: MongoDB Integration
Use MongoDB Atlas to store raw data.
Step 1: MongoDB Atlas Configuration
Sign up for MongoDB Atlas and create a new project.
Set up a free M0 cluster, configure the username and password, and allow access from any IP address (0.0.0.0/0).
Retrieve the MongoDB connection string for Python and save it (replace <password> with your password).
Step 2: Pushing Data to MongoDB
Create a folder named notebook, add the dataset, and create a notebook file mongoDB_demo.ipynb.
Use the notebook to push data to the MongoDB database.
Verify the data in MongoDB Atlas under Database > Browse Collections.

✅ Phase 3: Logging & Exception Handling
Implement centralized logging using logger.py.

Handle custom exceptions with exception.py.

✅ Phase 4: Data Pipeline (ETL)
Data Ingestion

Connect to MongoDB, retrieve datasets, and save locally.

Data Validation

Validate schema using schema.yaml.

Data Transformation

Clean and transform features for model input.

✅ Phase 5: Model Training & Evaluation
Use Scikit-learn models and transformers.

Evaluate models using thresholds defined in constants.

Save models as serialized .pkl objects using dill.

✅ Phase 6: AWS Integration
Upload trained models to AWS S3.

Use IAM roles and secure keys for access.

Store and version model artifacts in S3 buckets.

✅ Phase 7: Model Deployment
Build a FastAPI app to serve predictions.

Routes:

/ → Homepage

/predict → Vehicle insurance prediction

/train → Trigger model training pipeline

✅ Phase 8: CI/CD with GitHub Actions & AWS EC2
Setup GitHub Actions with AWS secrets.

Use Docker to containerize the application.

Use AWS EC2 (Ubuntu) as a self-hosted GitHub runner.

CI/CD flow:

Code pushed to GitHub.

GitHub Action triggers.

Docker image pushed to AWS ECR.

Image deployed to EC2 instance.

FastAPI app hosted on EC2 public IP (Port 5080).

🎯 Project Workflow Summary
Data Ingestion ➔ Data Validation ➔ Data Transformation
             ➔ Model Training ➔ Model Evaluation ➔ Model Deployment
             ➔ CI/CD Automation with GitHub Actions, Docker & AWS

---------------------------------------------------------------------
=======
>>>>>>> cfc24f98670431f053d6e525ebbe53ed271c5e0e
