# How to Run FastAPI on Another Computer

Step 1: Clone the Repository

If you are sharing this project via Git, others need to clone it first:

```bash
git clone <repository_url>
cd FastAPI
```

Step 2: Set Up a Virtual Environment

To create and activate a virtual environment:

For Windows (PowerShell):
```bash
python -m venv venv
.\venv\Scripts\activate
```
For macOS/Linux:
```bash
python3 -m venv venv
source venv/bin/activate
```

Step 3: Install Dependencies

Run the following command to install required packages:
```bash
pip install -r requirements.txt
```

Step 4: Run the FastAPI Application

Start the FastAPI server:
```bash
uvicorn main:app --reload
```

This will run the API at: http://127.0.0.1:8000

Step 5: Access the API Documentation
Once the server is running, access:

Swagger UI: http://127.0.0.1:8000/docs
ReDoc: http://127.0.0.1:8000/redoc
