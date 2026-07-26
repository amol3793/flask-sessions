# flask-sessions

A minimal Flask app demonstrating server-side session-based authentication (no database — for learning/demo purposes).

## Routes

| Route | Description |
|---|---|
| `/` | Login form (POST with `username`/`password` to sign in; the demo password is `password`) |
| `/protected` | Only accessible once a session is set; otherwise redirects to `/` |
| `/getsession` | Returns the logged-in username, or `Not logged in!` |
| `/dropsession` | Clears the session (log out) |

## Usage

```bash
pip install flask
python session.py
```

Then visit `http://localhost:5000`.

Walkthrough video: https://youtu.be/eBwhBrNbrNI
