#  **README.md — Smart Contract Status Dashboard**

##  Overview

**Smart Contract Status Dashboard** is a full-stack dApp that connects to deployed Ethereum smart contracts and provides **human-readable insights** into their live state. This tool makes it easy for anyone to **verify ownership, token details, paused state, and more**—without needing to navigate complex block explorers or decode ABI data.

##  Features

*  Enter any **Ethereum contract address**
*  View **contract metadata** (name, symbol, supply)
*  Check **paused status**
*  Display **contract owner**
*  Responsive **React.js frontend**
*  **FastAPI backend** using `web3.py`
*  Network support for **Ethereum Mainnet & Testnets (Goerli, Sepolia)**

##  Tech Stack

* **Frontend**: React.js, Axios
* **Backend**: Python FastAPI, web3.py
* **Blockchain**: Ethereum 

---

##  Project Structure

```
smart-contract-dashboard/
├── backend/
│   ├── app.py                # FastAPI server with web3.py contract interaction logic
│   ├── requirements.txt      # Python dependencies
│   └── utils.py              # Helper functions (ABI loading, connection handling)
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/       # Reusable React components (StatusCard, InputForm, etc.)
│   │   ├── pages/            # Main pages like Dashboard.jsx
│   │   ├── api/              # Axios API client setup
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── package.json          # Frontend dependencies
│   └── README.md             # Frontend-specific notes
│
└── README.md                 # Project overview (this file)
```

---

##  Local Development Setup

### 1. Clone the Repository

```bash
git clone https://github.com/sgtanvi/smart-contract-dashboard.git
cd SmartContract
```

### 2. Backend Setup

```bash
cd backend
python -m venv venv
.\venv\Scripts\activate  # Windows
# source venv/bin/activate  # Mac/Linux
pip install -r requirements.txt
uvicorn app:app --reload
```

### 3. Frontend Setup

```bash
cd ../frontend
npm install
npm run dev
```

---

##  Example Usage

1. Open the frontend at host
2. Enter a **smart contract address** (e.g., an ERC20 contract)
3. View:

   *  Owner address
   *  Paused status
   *  Token supply
   *  Contract name and symbol

---

## Roadmap

* [ ] Multi-network support (Polygon, BSC)
* [ ] Contract function explorer
* [ ] Transaction history viewer
* [ ] Wallet connection for privileged views

---


## License

[MIT](LICENSE)

