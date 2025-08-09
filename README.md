# Medical_Records_Miniproject

# Medical Report Management

##  Overview  
**Medical Report Management** is a decentralized mini-project that enables hospitals, doctors, and patients to manage and record medical reports using Solidity smart contracts. The front-end interfaces (HTML) interact with these contracts to enable transparent and secure access management.

---

##  Features & Functionality  
- **Solidity Smart Contracts** (`.sol`) for:
  - Managing patient records
  - Recording examinations
  - Managing doctor–hospital details
- **Front-End (HTML):**
  - Doctor registration and detail forms
  - Examination record entry and detail views
  - Patient and hospital interfaces for seamless interaction

---

##  Folder Structure

```

MEDICAL\_REPORT\_MANAGEMENT/
├── README.md
├── \_config.yml               # (Optional project configuration)
├── doctor.sol                # Smart contract for doctor info
├── patient.sol               # Smart contract for patient data
├── records.sol               # Smart contract for medical records
├── body\_examine.sol          # Contract defining examination details
├── HTML Interfaces:
│   ├── doctor.html
│   ├── doctor\_details.html
│   ├── patient.html
│   ├── patient\_details.html
│   ├── patient\_examine.html
│   ├── examine\_details.html
│   ├── hospital.html
│   ├── hospital\_details.html
│   └── record.html
│   └── record\_details.html

````

---

##  Getting Started

###  Prerequisites
- **Node.js / npm** — for package management and scripts  
- **Truffle** or **Hardhat** — for compiling and deploying contracts  
- **Ganache** or another local Ethereum network  
- Browser with **Metamask** to connect with smart contracts

###  Setup & Run
1. **Clone the repository**
   ```bash
   git clone https://github.com/MahendraSN/MEDICAL_REPORT_MANAGEMENT.git
   cd MEDICAL_REPORT_MANAGEMENT
````

2. **Compile Solidity contracts**

   * Using Truffle:

     ```bash
     truffle compile
     ```
   * Or Hardhat:

     ```bash
     npx hardhat compile
     ```

3. **Deploy contracts to local blockchain**

   * Truffle:

     ```bash
     truffle migrate --network development
     ```

4. **Launch front-end**

   * Open each HTML file using a browser.
   * Connect MetaMask to your local Ethereum network (e.g. localhost:8545).

---

## Usage & Workflow

1. **Registration Interfaces**:

   * Use `doctor.html` or `patient.html` to register respective entities via smart contracts.

2. **Entering Details**:

   * Register hospitals through `hospital.html`.
   * Add examination records with `patient_examine.html`.

3. **Viewing Records**:

   * Query and display doctor, patient, hospital, or medical record details using respective HTML pages like `doctor_details.html`, `record_details.html`, etc.

4. **Smart Contract Interaction**:

   * Each HTML interface triggers contract functions (e.g., `addDoctor()`, `addPatient()`, `recordExamination()`).

---

## Potential Enhancements

* Integrate **IPFS** to offload and manage medical report files (PDFs/images)
* Add **user authentication** (e.g. via Ethereum accounts or tokens)
* Enhance UI using **React** or **Vue.js**
* Develop **automated tests** for smart contracts

---

