mkdir backend && cd backend
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install fastapi uvicorn
uvicorn main:app --reload --port 8002


Deploy
Push to GitHub and connect to Render:
Go to render.com
Click “New Web Service”
Choose Python
Set uvicorn main:app as the Start Command
Done!