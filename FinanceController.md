# 1. GET all transactions
* GET
* path: ```/api/finance/all```
* Required role: ```"ROLE_FARM_OWNER"```
* Example body: NONE

<img width="400" alt="Zrzut ekranu 2024-10-13 o 18 53 59" src="https://github.com/user-attachments/assets/a589a0b2-1ea9-4414-ad88-46c8e0bf7ae5">

# 2. Add new transaction
* POST
* path: ```/api/finance/new```
* Required role: ```"ROLE_FARM_OWNER"```
* Example body:

```json
{
    "transactionName": "Transakcja8",
    "financialCategory": "EXPENSE",
    "paymentStatus": "UNPAID",
    "transactionDate": "2024-10-10",
    "paymentDate": "2024-10-17",
    "amount": 123,
    "description": "Test123"
}
```
<img width="400" alt="Zrzut ekranu 2024-10-13 o 18 53 26" src="https://github.com/user-attachments/assets/b3235265-0910-45a8-a64c-f24bd349a0f4">

# 3. Update transaction
* PUT
* path: ```/api/finance/{id}```
* Required role: ```"ROLE_FARM_OWNER"```
* Example body:

```json
{
    "transactionName": "Transakcja9",
    "financialCategory": "INCOME",
    "paymentStatus": "UNPAID",
    "transactionDate": "2024-10-10",
    "paymentDate": "2024-10-17",
    "amount": 1235,
    "description": "Test123"
}
```

<img width="400" alt="Zrzut ekranu 2024-10-13 o 18 53 34" src="https://github.com/user-attachments/assets/1a0cbec1-9869-48c3-b6f0-551e83ab228e">

# 4. Delete transaction
* DELETE
* path: ```/api/finance/{id}```
* Required role: ```"ROLE_FARM_OWNER"```
* Example body: NONE
  
<img width="400" alt="Zrzut ekranu 2024-10-13 o 18 53 40" src="https://github.com/user-attachments/assets/3e42385c-022a-4cff-abb1-425795240a5f">

# 5. Get farm finance balance
* GET
* path: ```/api/finance/balance```
* Required role: ```"ROLE_FARM_OWNER"```
* Example body: NONE
  
<img width="400" alt="Zrzut ekranu 2024-10-13 o 18 56 03" src="https://github.com/user-attachments/assets/99bcdb10-be7e-4af9-a7a9-543dd7114df3">

  
  
