# 1. GET all farm equipment
* GET
* path: ```/api/equipment/all```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE
* Request param:
  - Optional string: ```searchQuery```
 
<img width="400" alt="Zrzut ekranu 2024-10-1 o 20 17 08" src="https://github.com/user-attachments/assets/2d603c16-0a9e-4bb2-b47e-0116c5bc9a91">


# 2. GET farm equipment details
* GET
* path: ```/api/equipment/{equipmentId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE

<img width="400" alt="Zrzut ekranu 2024-10-1 o 20 15 25" src="https://github.com/user-attachments/assets/0bae42e0-8b83-494a-b468-9c7c560f96aa">

# 3. ADD farm equipment
* POST
* path: ```/api/equipment/new```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body:
  ```json
{
    "equipmentName": "Ładowarka Komatsu",
    "category": "Ładowarki kołowe",
    "brand": "Komatsu",
    "model": "265",
    "power": 265,
    "insurancePolicyNumber": "PL220023",
    "insuranceExpirationDate": "2027-04-04",
    "inspectionExpireDate": "2026-04-16"
}
  ```

<img width="400" alt="Zrzut ekranu 2024-10-6 o 14 29 23" src="https://github.com/user-attachments/assets/ffcb6611-9eb4-43d1-8d5c-c57a66477c9e">


# 3. UPDATE farm equipment details
* PUT
* path: ```/api/equipment/{equipmentId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body:
  ``` json
{
    "equipmentName": "Ładowarka Komatsu",
    "brand": "Komatsu",
    "model": "265 DI",
    "power": 265,
    "capacity": null,
    "workingWidth": null,
    "insurancePolicyNumber": "400429",
    "insuranceExpirationDate": "2027-05-20",
    "inspectionExpireDate": "2026-04-20"
}
  ```
<img width="400" alt="Zrzut ekranu 2024-10-5 o 18 16 29" src="https://github.com/user-attachments/assets/2031c67d-89a8-401f-82a9-38355867204d">

# 4. DELETE farm equipment
* DELETE
* path: ```/api/equipment/{equipmentId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE

  <img width="400" alt="Zrzut ekranu 2024-10-6 o 14 30 03" src="https://github.com/user-attachments/assets/71113164-dba0-49eb-999e-2223303b309f">


# 5. GET all equipment categories with data fields
* GET
* path: ```/api/equipment/categories```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER``` 
* Example body: NONE

  <img width="400" alt="Zrzut ekranu 2024-10-5 o 13 34 19" src="https://github.com/user-attachments/assets/242d0196-14d9-42fe-8474-d48595ceb709">

