# GoogleLoginWeb
Minimal Flask app for Google OAuth login using Authlib.

## Setup
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
```

Fill `.env`:
```
GOOGLE_CLIENT_ID=...
GOOGLE_CLIENT_SECRET=...
GOOGLE_OAUTH_REDIRECT_URL=http://localhost:5000/auth/google/callback
FLASK_SECRET_KEY=...
```

## Run
```bash
python app.py
```
Open http://localhost:5000

## Notes
- `AUTHLIB_INSECURE_TRANSPORT=1` is enabled for HTTP in dev. Use HTTPS in production.
