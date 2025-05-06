# Django Chat App

A simple real-time chat application built using Django and AJAX. Users can join rooms and exchange messages in real time through a dynamic interface.

## Features

* Join or create chat rooms on the fly
* Real-time messaging with AJAX (no page reloads)
* `home.html` for room entry, `room.html` for chat interface
* Room and Message models to store chat data
* Clean and minimal UI

## Tech Stack

* Python
* Django
* SQLite (default Django DB)
* JavaScript (AJAX via jQuery or Fetch API)
* HTML/CSS

## How It Works

1. User visits the home page (`home.html`) and enters a room name.
2. They're redirected to `room.html` where the chat takes place.
3. Messages are sent and received via AJAX, which calls Django views that handle saving and retrieving messages.
4. JavaScript periodically polls the server for new messages, simulating real-time behavior.

## Getting Started

### Prerequisites

* Python 3.x
* pip

### Setup

```bash
# Clone the repository
git clone https://github.com/GiorgiEz/Chat-App-Django.git
cd Chat-App-Django

# Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Run the server
python manage.py runserver
```

Visit `http://127.0.0.1:8000/` to start chatting!

## To Do

* Add user authentication (login/logout)
* Implement WebSockets with Django Channels for better real-time experience
* Add timestamps, usernames, and better styling
* Improve performance with message pagination or throttling
