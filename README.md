# 🧮 Advanced Calculator Microservice

This project is a Node.js-based calculator microservice that supports both basic and advanced arithmetic operations via REST API endpoints. It includes detailed logging and input validation.

---

## ✅ Features Implemented

- ➕ Addition (`/add`)
- ➖ Subtraction (`/subtract`)
- ✖️ Multiplication (`/multiply`)
- ➗ Division (`/divide`)
- 🧮 Modulo (`/mod`)
- ⚡ Power (`/power`)
- √ Square Root (`/sqrt`)
- 🔁 Unified route (`/calculate`) with operation selector

---

## 🛠️ Technologies Used

- [Node.js](https://nodejs.org)
- [Express.js](https://expressjs.com)
- [Winston](https://github.com/winstonjs/winston) (logging)
- Postman (for API testing)
- Git + GitHub
- Docker (optional)

---

## 📦 Installation and Setup

```bash
# Clone the repository
git clone https://github.com/<your-username>/sit323-2025-prac4c.git
cd sit323-2025-prac4c

# Install dependencies
npm install

# Run the microservice
node cal.js

## App will run at:
http://localhost:3051
---

## 🌐 API Endpoints

| Method | Endpoint     | Description                          |
|--------|--------------|--------------------------------------|
| GET    | `/add`       | Add two numbers                      |
| GET    | `/subtract`  | Subtract two numbers                 |
| GET    | `/multiply`  | Multiply two numbers                 |
| GET    | `/divide`    | Divide two numbers                   |
| GET    | `/power`     | Exponentiation                       |
| GET    | `/mod`       | Modulo of two numbers                |
| GET    | `/sqrt`      | Square root of a number              |
| GET    | `/calculate` | General operation using query param  |

---

## 🧪 Example API Calls

GET /add?n1=10&n2=5
GET /mod?n1=15&n2=4 GET /sqrt?n1=25
GET /calculate?n1=2&n2=3&operation=power


---

## 🐳 Docker (Optional)

### Dockerfile
```Dockerfile
FROM node:18
WORKDIR /app
COPY . .
RUN npm install
EXPOSE 3051
CMD ["node", "cal.js"]
Build & Run
docker build -t calculator-microservice .
docker run -p 3051:3051 calculator-microservice
📂 Project Structure

├── cal.js               # Main server file
├── package.json         # Node dependencies
├── error.log            # Error log
├── combined.log         # Info + error log
├── Dockerfile           # (Optional) Containerization
└── README.md            # Documentation
