# RealEstate Booking (JS Only)

- contracts/: Hardhat (JS), Solidity contract, deploy and tests
- backend/: Express + MongoDB + JWT, contract integration via ethers
- frontend/: React + Vite + Tailwind, routing and placeholders

Setup (Windows PowerShell):

1) Contracts
- cd contracts
- npm install
- create .env with MUMBAI_RPC_URL, PRIVATE_KEY, POLYGONSCAN_API_KEY
- npx hardhat compile
- npm test
- npx hardhat run scripts/deploy.js --network mumbai

2) Backend
- cd backend
- npm install
- create .env with MONGO_URI, JWT_SECRET, CONTRACT_ADDRESS, MUMBAI_RPC_URL, PRIVATE_KEY
- npm run dev

3) Frontend
- cd frontend
- npm install
- npm run dev
