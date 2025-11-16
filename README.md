
QuickChat — Python Live Chat App

  

Modern, minimal real-time chat application built with Flask and WebSockets. QuickChat demonstrates a clean, production-minded Flask app structure, live messaging with Socket.IO, and simple templates for easy customization.

  

Key goals:

  

-  Provide a small, focused example of real-time web features.

-  Show practical use of Flask + Socket.IO in a lightweight codebase.




##  Demo

  

Try a quick demo of the app by clicking [here](https://quickchatpython.onrender.com).

Screenshots:
![HomePage](/assets/home.PNG "Home Page")

![Live Room](/assets/room.PNG "Live Room")


  

##  Highlights

  

-  Real-time messaging using WebSockets (Flask + Socket.IO)

-  Multi-room chat support (via separate URLs/templates)

-  Simple, responsive UI built with HTML/CSS (located in `templates/` and `static/`)

  

##  Tech Stack

  

-  Python 3.8+ (tested)

-  Flask

-  Flask-SocketIO (or python-socketio)

-  HTML/CSS (templates & static assets)

  

##  Getting Started 

  

These instructions assume you're on Windows PowerShell . Adjust commands for macOS / Linux shells.

  

1. Create and activate a virtual environment

  

```powershell

python -m venv .venv

.\.venv\Scripts\Activate.ps1

```

  

2. Install dependencies

  

```powershell

pip install -r requirements.txt

```

  

3. Create a `.env` file in the project root . At minimum, configure a secret key and optional dev flags:

  

```env

SECRET_KEY="Your_KEY"

PORT=5000

```

  

4. Run the app locally

  

```powershell

python main.py

```

  

5. Open your browser at `http://localhost:5000` (or the `PORT` you configured). Open multiple browser windows to test real-time messaging.

  



##  Structure Overview

  

-  `main.py` — application entrypoint and server runner

-  `templates/` — Jinja2 templates: `base.html`, `home.html`, `room.html`

-  `static/` — CSS and static assets

  


  

##   Next Steps 

  

-  Add user authentication (Flask-Login) and per-user message history.

-  Persist messages to a lightweight DB (SQLite) and paginate conversation history.

-  Add end-to-end tests and CI (GitHub Actions).

  

