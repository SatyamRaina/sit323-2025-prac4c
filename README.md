This project implements a Node.js-based microservice calculator that supports basic and advanced operations via REST API.

✅ Features Implemented
Addition (/add)
Subtraction (/subtract)
Multiplication (/multiply)
Division (/divide)
Power (/power)
Modulo (/mod)
Square root (/sqrt)
Unified route with /calculate?operation=...

📦 Technologies Used
Node.js
Express
Winston (Logging)
Docker (optional)

🛠️ How to Run
npm install
node cal.js

The app will start at:
http://localhost:3051

📬 Sample API Requests
GET /calculate?n1=10&n2=2&operation=divide

GET /sqrt?n1=25

GET /mod?n1=10&n2=3
