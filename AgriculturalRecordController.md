# 1. GET all records per season
* GET
* path: ```/api/records/all```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"``` or ```"ROLE_FARM_EQUIPMENT_OPERATOR"```
* Example body: NONE
* Request param:
  - Optional String: ```season```
  - Optional String: ```searchQuery```

<img width="400" alt="Zrzut ekranu 2024-10-25 o 20 51 25" src="https://github.com/user-attachments/assets/d6159e3c-ce42-4e69-8e74-e3b6be83eec6">


# 2. Add new record for landparcel (second crop)
* POST
* path: ```/api/records/add-new-record```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body:

```json
{
    "cropName": "arbuz",
    "area": 10,
    "season": "2026/2027",
    "landparcelId": 4
}
```
<img width="400" alt="Zrzut ekranu 2024-10-25 o 20 51 38" src="https://github.com/user-attachments/assets/dd1a58a2-3607-4e7a-8af7-9400db816aeb">

# 3. Add records for new season
* POST
* path: ```/api/records/generate-records-for-new-season```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE
* Request Params:
  - Required String: ```seasonName```

 
  <img width="400" alt="Zrzut ekranu 2024-10-26 o 23 11 13" src="https://github.com/user-attachments/assets/61140ed3-bff8-46ee-bcba-ad10b6e93a77">

# 4. Update agriculture record
* PUT
* path: ```/api/records/add-new-record```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body:
```json
{
    "cropName": null,
    "area": 0.04,
    "description": null
}
```

<img width="400" alt="Zrzut ekranu 2024-10-25 o 20 51 48" src="https://github.com/user-attachments/assets/a5ca5222-6d18-4f31-bd72-19ff8835a806">


# 5. Get available seasons
* GET
* path: ```/api/records/available-seasons```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE

<img width="400" alt="Zrzut ekranu 2024-10-25 o 20 51 58" src="https://github.com/user-attachments/assets/bd13b7a3-51cd-42af-9b32-dade1751506e">

# 6. Get available crops
* GET
* path: ```/api/records/available-crops```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE

<img width="400" alt="Zrzut ekranu 2024-10-25 o 20 52 05" src="https://github.com/user-attachments/assets/73268049-3c7f-4da8-a5cc-87ea0f27c8c8">

