🏦 Bank Management System (Streamlit App)

A Bank Management System built using Python and Streamlit that allows users to create accounts, manage balances, and transfer money between accounts and banks.

This project simulates basic banking operations with JSON-based storage, providing a clean UI and interactive experience using Streamlit.

---

📌 Features

👤 Account Management

- Create a new bank account
- View account details
- Update account details
- Delete account permanently

💰 Transaction Features

- Deposit money
- Withdraw money
- Transfer money to another account

🔄 Money Transfer

1. Account → Account Transfer (Same Bank)
2. Bank → Bank Transfer (Different Banks)

🔐 Security

- PIN based authentication
- Unique account number generation
- Balance validation before withdrawal/transfer

💾 Data Storage

All data is stored locally using JSON files, simulating a simple banking database.

---

🗂 Project Structure

Bank Management System
│
├── app.py              # Main Streamlit application
├── main.py         # Terminal version of the banking system
│
├── data.json           # Main bank database
├── sbi.json            # SBI bank database
├── pnb.json            # PNB bank database
├── indian.json         # Indian Bank database
├── canera.json         # Canera Bank database
├── bob.json            # Bank of Baroda database
│
└── README.md

---

⚙️ Technologies Used

- Python
- Streamlit
- JSON
- Random & String Modules
- Pathlib

---

🚀 Installation & Setup

1️⃣ Clone the Repository

git clone https://github.com/Pranay-256/DATA-SCIENCE-PROJECTS.git

2️⃣ Navigate to the Project Folder

cd DATA-SCIENCE-PROJECTS/Python Projects/Bank Management System

3️⃣ Install Required Libraries

pip install streamlit

---

▶️ Run the Application

Start the Streamlit app using:

streamlit run app.py

Your browser will open automatically with the banking interface.

---

🖥 Streamlit UI Features

The Streamlit interface includes:

- 📌 Sidebar navigation menu
- 🎨 Styled UI elements
- 🔐 Secure PIN based login
- 💰 Real-time balance updates
- 💸 Account to account transfers

---

📊 Example Banking Operations

✔ Create Account
✔ Deposit Money
✔ Withdraw Money
✔ View Details
✔ Update Details
✔ Delete Account
✔ Send Money

---

📚 Learning Outcomes

This project helped in understanding:

- Building interactive web apps using Streamlit
- Handling JSON as a lightweight database
- Implementing authentication systems
- Managing financial transactions logic
- Designing clean UI dashboards

---

👨‍💻 Author

Pranay Jha

Aspiring Data Analyst / Data Science Enthusiast

GitHub:
https://github.com/Pranay-256

---

⭐ If you found this project useful, consider giving the repository a star.
