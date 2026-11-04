# NIRF Chatbot

## Run the Streamlit dashboard

With Streamlit and the backend dependencies installed, configure the required
`DATABASE_URL` and `SARVAM` environment variables in the repository-root
`.env` file (or in the process environment), then run the dashboard from this
directory:

```powershell
python -m pip install -r ..\requirements.txt
streamlit run streamlit_app.py
```

The chatbot source package is resolved relative to this project, and database
settings are loaded from the repository-root `.env` regardless of the current
working directory. The dashboard keeps a chat history and presents each answer
with result, chart, SQL, and plotting-code tabs. Generated plotting code is
displayed for review and is never executed by the dashboard.
