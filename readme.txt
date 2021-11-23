SmartLoans on Blockchain is divided into 4 independent projects:
a)Add Asset
b)Add Loan
c)Lend Loan
d)Repay Loan

These 4 projects are run simultaneously on different ports using the below command:
ng serve --port port_no

Attached zip file contains the source code for the 4 projects and the contracts. Extract the contents prior to proceeding with the setup. Smart contracts contains the contracts(/contracts) as well as the migration scripts(/migration). Rename the .txt files present in migrations folder to .js



Steps to run the project:
1)Create a folder for the project, say AddAsset
2)Create an src folder inside AddAsset. Copy the extracted contents for the appropriate project and paste it in ur created /src.
3)Copy the contracts folder,migrations folder, package.json, package-lock.json, tsconfig.json in your project folder
4)Open cmd in that project folder and do  npm install
5)Post npm install, do an ng serve to load the project
6)Follow the above steps for the remaining 3 projects


For contract deployment:
1)Compile and deploy RealEstateBeta,RealEstatePrices and Repayment by opening a cmd prompt in the Smart Contracts folder(copied from the extracted files).Ensure migration and contract folders are in the same parent directory
2)Copy the addresses generated for RealEstateBeta & RealEstatePrices and paste them in the Migration file for smartloanBeta. RealEstatePrices address will also be pasted in the python script
3)Run the python script
4)Deploy SmartLoanBeta

Command for compiling and deploying specific contracts
truffle migrate --compile-all -f 2 --to 2 //where 2 is the contract number present on the migration js file for that contract

Tools used:
1)node
2)truffle
3)Ganache
4)Metamask
5)Python 3.6
