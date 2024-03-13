# ChiaLoans: Blockchain-Based Loan Management System (Beginner Category)

ChiaLoans is a beginner-friendly application that leverages blockchain technology to manage loans efficiently. Below, we outline the key components of ChiaLoans and provide instructions for setting up and deploying the smart contracts.

## Application Components:
1. Add Asset:
    - Allows users to add assets (collateral) that can be used to secure loans.
    - Asset details, such as type, value, and ownership, are recorded on the blockchain.

2. Add Loan:
    - Users can create loan requests by specifying the loan amount, interest rate, and collateral.
    - The smart contract ensures transparency and security during the loan creation process.

3. Lend Loan:
    - Lenders can review available loan requests and choose to fund them.
    - Funds are transferred to the borrower's account, and the loan terms are enforced by the smart contract.

4. Repay Loan:
    - Borrowers can repay their loans by transferring the agreed-upon amount.
    - The smart contract tracks repayments and updates the loan status accordingly.

## Setup Instructions:
1. Extract Contents:
    - Download the attached zip file containing the source code for ChiaLoans.
    - Extract the contents to a local directory.

2. Project Setup:
    - Create a separate folder for each project component (e.g., AddAsset, AddLoan, LendLoan, RepayLoan).
    - Inside each project folder, create an `src` directory.
    - Copy the relevant extracted contents into the respective `src` folders.

3. Smart Contracts:
    - Copy the `contracts` folder and the `migrations` folder from the extracted files.
    - Also, copy `package.json`, `package-lock.json`, and `tsconfig.json` to your project folder.

4. Install Dependencies:
    - Open a command prompt in each project folder.
    - Run `npm install` to install the necessary dependencies.

5. Run the Projects:
    - Execute `ng serve --port port_no` for each project (replace `port_no` with the desired port number).
    - This will run the projects simultaneously on different ports.

6. Contract Deployment:
    - Compile and deploy the following smart contracts:
        - RealEstateBeta
        - RealEstatePrices
        - Repayment
    - Ensure that the migration and contract folders are in the same parent directory.
    - Copy the addresses generated for RealEstateBeta and RealEstatePrices and paste them in the Migration file for SmartLoanBeta.
    - The RealEstatePrices address should also be included in the Python script.
    - Run the Python script to finalize the deployment.
    - Deploy SmartLoanBeta using the appropriate command (e.g., `truffle migrate --compile-all -f 2 --to 2`).

## Tools Used:
1. Node: JavaScript runtime environment.
2. Truffle: Development framework for Ethereum smart contracts.
3. Ganache: Local blockchain simulator for testing.
4. Metamask: Ethereum wallet and browser extension.
5. Python 3.6: Used for additional deployment tasks.

*Feel free to explore ChiaLoans and start managing loans on the blockchain! 🔗
