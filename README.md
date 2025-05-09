# Django Channels Basic Chat

A simple real-time chat application built with Django and Django Channels.

## Features

- Real-time messaging using WebSockets
- Multiple chat rooms support
- Simple and clean user interface

## Requirements

- Python 3.x
- Django
- Django Channels
- Channels Redis (for production)

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dhirajdurgade7758/django-channels-basic-chat.git
   cd django-channels-basic-chat
   
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate

   pip install -r requirements.txt
   python manage.py migrate
   python manage.py runserver
   ```

2. **Access the app:**
   Open your browser and go to:
   ```
   http://127.0.0.1:8000/
   ```

## Project Structure

```
django-channels-basic-chat/
├── chat/               # Django app containing chat logic and consumers
│   ├── consumers.py
│   ├── models.py
│   ├── routing.py
│   ├── views.py
│   ├── templates/
│   │   └── chat/
│   │       └── room.html
├── mysite/             # Project configuration and ASGI setup
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
├── manage.py
├── requirements.txt
└── README.md
```

## License

This project is for educational purposes.