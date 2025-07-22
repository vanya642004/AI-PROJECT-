# AI‑Agent for E‑commerce Data

**What:**  
A Flask + SQLite backend + LLM agent that turns natural‑language questions into SQL queries on your ad_sales, total_sales & eligibility tables, plus a vanilla HTML/JS frontend.

**Quick Start (no CLI):**  
1. Click **Code → Open with Codespaces → New codespace**  
2. Wait—the devcontainer will install deps, load CSVs, and start:  
   - **Backend (Flask API):** http://localhost:5000  
   - **Frontend (Static site):** http://localhost:3000  
3. Ask things like “What is my total sales?”, “Which product has highest CPC?”  

**Local (CLI) alternative:**  
```bash
cd backend
pip install -r requirements.txt
python load_data.py      # builds ecom.db
python app.py            # launches API on :5000
# in another shell:
cd ../frontend
python -m http.server 3000
