# TrustLens - Fake News Detector

### Project Overview
TrustLens is a comprehensive platform designed to detect, combat, and prevent the spread of misinformation across various media formats. The solution employs machine learning models for real-time fake news detection in text, image, and video content. TrustLens provides users with real-time fact-checking capabilities and allows journalists to register, verify their articles, and claim ownership via a blockchain-powered decentralized application (Dapp). The project is a full-stack solution that includes mobile, browser extension, and blockchain-based features for verifiable content ownership.

### Problem Statement
In an era where misinformation spreads rapidly across digital platforms, there is an urgent need to combat fake news efficiently. Current methods of detecting fake news are either too slow or ineffective across different content formats. Additionally, journalists often face challenges in proving the authenticity and ownership of their work. TrustLens addresses these challenges by providing an automated, multi-media, fake news detection system and a blockchain-based proof-of-ownership mechanism for journalists, ensuring transparency, authenticity, and trust in the information being shared.

### Deliverables
1. **Fake News Detection Models**:
   - Machine learning models to detect fake news in text, image, and video content.
   - Models designed without the use of external API keys for verification, keeping the system self-contained.
   - Cross-referencing facts for real-time fact-checking.
   
2. **Browser Extension**:
   - Real-time analysis of web content, articles, and media on websites.
   - Integration with the backend for misinformation detection and suggestion of alternative news sources.
   
3. **Mobile Application**:
   - A mobile app for scanning content (text or images) and receiving real-time fact-checking results.
   - Cross-platform support for Android and iOS.
   - Efficient media processing for real-time responses.
   
4. **Admin Panel**:
   - A web-based admin interface for monitoring reported content and user activity.
   - System for reviewing and flagging mass-reported fake news.
   - Proof of concept for custom image analysis and backend database management.

5. **Blockchain-Based Ownership Verification**:
   - A decentralized application (Dapp) for journalists to claim ownership of their published articles.
   - Timestamping articles to ensure the originality and prevent plagiarism.
   - Public ledger to verify article metadata, ownership, and publication timestamp.
   - Proof-of-concept implementation to showcase functionality.

### Tech Stack
The project utilizes a diverse tech stack to ensure the solution is robust, scalable, and efficient:

- **Frontend**:
  - **React**: A modern JavaScript library for building responsive and interactive user interfaces.
  - **Tailwind CSS**: A utility-first CSS framework for styling, offering a sleek, sci-fi/gaming-inspired UI design.
  - **React Native with Expo**: For developing the mobile application across both Android and iOS platforms.
  - **Metamask Integration**: Provides easy access to blockchain features for users, such as wallet connections and smart contract interactions.

- **Backend**:
  - **FastAPI**: A high-performance Python framework for building APIs, used for handling the backend services.
  - **SQLAlchemy & SQLite**: Database management for storing article records, user details, and reports.
  - **Machine Learning (scikit-learn)**: For building and deploying fake news detection models.


- **Blockchain**:
  - **Solidity**: Smart contracts for blockchain-based article timestamping and ownership verification.
  - **Ethereum & ERC721 (NFT Standard)**: Used for creating non-fungible tokens (NFTs) that represent article ownership.
  - **Truffle**: For compiling, testing, and deploying the smart contracts.
  - **Ganache**: For local blockchain development and testing.

### Deliverables

1. **Fake News Detection**
   - Machine learning models for text, image, and video analysis.
   - Data preprocessing and model training.
   - No external API integration.

2. **Browser Extension**
   - Real-time content analysis in browser.
   - Backend integration for fake news detection and fact-checking.

3. **Mobile App Development**
   - Cross-platform mobile app for content verification.
   - Backend support for media processing.

4. **Admin Panel**
   - Web interface for monitoring mass-reported articles.
   - Custom image analysis for fake news detection (proof-of-concept).

5. **Blockchain-Based Ownership Verification**
   - Dapp for timestamping and verifying content ownership.
   - ERC721 standard for minting NFTs as ownership proof.
   - Integration of journalist verification and public article showcase.

### Dummy JSON for Metadata (Used in Smart Contract)
```json
{
  "title": "The Future of Decentralized Journalism",
  "description": "An in-depth look at how blockchain technology is transforming journalism.",
  "author": "Jane Doe",
  "content": "Lorem ipsum dolor sit amet, consectetur adipiscing elit...",
  "publicationDate": "2024-10-19",
  "image": "https://example.com/image.jpg",
  "tags": ["blockchain", "journalism", "decentralization"]
}
```

### Installation and Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Vivaangarg16/trustlens.git
   cd trustlens
   ```

2. **Frontend**:
   - Navigate to the frontend directory:
     ```bash
     cd frontend
     npm install
     npm run dev
     ```
   - Ensure Metamask is installed and connected.

3. **Backend**:
   - Navigate to the backend directory:
     ```bash
     cd backend
     pip install -r requirements.txt
     uvicorn main:app --reload
     ```
   
4. **Smart Contract Deployment**:
   - Compile and deploy smart contracts using Truffle:
     ```bash
     cd blockchain
     truffle compile
     truffle migrate --network development
     ```

5. **MetaMask**:
   - Ensure MetaMask is installed in your browser.
   - Connect to the appropriate network (Ganache for development or any testnet/mainnet for production).

### Summary
TrustLens offers a state-of-the-art, multi-faceted solution to combat misinformation through real-time detection of fake news and blockchain-based verification of article ownership. With its robust tech stack and future-proof features, the platform empowers both the public and journalists to detect and prevent the spread of false information.

