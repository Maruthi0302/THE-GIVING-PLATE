# 🍽️ THE GIVING PLATE

Connecting food donors (Givers) with those in need (Receivers) using smart matching and geolocation. Built with Flask, MySQL, and SQLAlchemy.

---

## ✨ Features

- 🥗 Register as a food Giver or Receiver
- 🤝 Smart matching based on food type, dietary needs, and location
- 🔗 RESTful API endpoints
- 🗄️ MySQL database backend
- 🖥️ Simple web interface (HTML/CSS/JS)

---

## 🚀 Getting Started

### Prerequisites

- 🐍 Python 3.7+
- 🐬 MySQL Server

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Maruthi0302/THE-GIVING-PLATE.git
   cd THE-GIVING-PLATE
   ```

2. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the MySQL database**
   - Start your MySQL server.
   - Create a database named `food_db`:
     ```sql
     CREATE DATABASE food_db;
     ```
   - Import the schema:
     ```bash
     mysql -u root -p food_db < schema.sql
     ```
   - _(Default MySQL credentials are set in `database.py` as `root`/`MySQL123$`. Change as needed.)_

4. **Run the Flask app**
   ```bash
   python app.py
   ```
   - The app will be available at [http://127.0.0.1:5000/](http://127.0.0.1:5000/)

---

## 📡 API Endpoints

- `POST /giver` — Register a new food Giver
- `GET /givers` — List all Givers
- `GET /giver/<id>` — Get a Giver by ID
- `POST /receiver` — Register a new Receiver and get best match
- `GET /receivers` — List all Receivers
- `GET /receiver/<id>` — Get a Receiver by ID

---

## 🗂️ Project Structure

```
.
├── app.py
├── routes.py
├── database.py
├── models.py
├── ai_matching.py
├── requirements.txt
├── schema.sql
├── givng Plate/
│   └── (HTML, CSS, JS, PHP files for web interface)
└── Nearbyplaces/
    └── (Additional resources)
```

---

## 🤗 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙏 Acknowledgements

- Flask
- SQLAlchemy
- MySQL
- geopy

---

> Made with ❤️ for the community!
