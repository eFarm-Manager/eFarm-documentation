# 1. Add New Agro Activity
* POST
* path: ```/api/agro-activities/new```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body:

```json
{
    "name": "Oprysk nr 2",
    "activityCategoryName": "Opryskiwanie herbicydami",
    "date": "2024-11-01T10:00:00Z",
    "isCompleted": true,
    "usedSubstances": "Corteva Navigator 360SL",
    "appliedDose": " 2,5 L/ha",
    "description": "Wystąpiły chwasty na terenach podmokłych",
    "agriculturalRecordId": 5,
    "operatorIds": [1, 2],
    "equipmentIds": [3, 4]
}
```

![Screenshot from 2024-11-05 21-27-12](https://github.com/user-attachments/assets/6c8f9ddc-f4d6-4bd6-988a-eb543d9008e0)

# 2. Get Agro Activities list for agricultural record
* GET
* path: ```/api/agro-activities/{agriculturalRecordId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE
* Request param: NONE

<img width="400" alt="Zrzut ekranu 2024-11-7 o 13 43 34" src="https://github.com/user-attachments/assets/497a8a29-3889-4e8e-8958-2d7ac465b8c0">


# 3. Get Agro Activity details
* GET
* path: ```/api/agro-activities/details/{agroActivityId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER``` or ```ROLE_FARM_EQUIPMENT_OPERATOR```
* Example body: NONE
* Request param: NONE


<img width="400" alt="Zrzut ekranu 2024-11-7 o 13 45 44" src="https://github.com/user-attachments/assets/f72c694f-3cb6-4dae-a13c-c1542b59127b">


# 4. Update Agro Activity
* PUT
* path: ```/api/agro-activities/{agroActivityId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body:

```json
{
    "name": "Oprysk chwastobójczy numer 3",
    "activityCategoryName": "Opryskiwanie herbicydami",
    "date": "2024-11-06T11:26:00.254429Z",
    "isCompleted": true,
    "usedSubstances": "Corteva Navigator 360SL",
    "appliedDose": " 3,5 L/ha",
    "description": "Na polach występuje wiele chwastów",
    "operatorIds": [6, 14, 24],
    "equipmentIds": [2, 4]
}
```

<img width="400" alt="Zrzut ekranu 2024-11-8 o 18 30 43" src="https://github.com/user-attachments/assets/75f1c4cc-905d-446f-b6a5-8dd614507aa3">

# 5. Delete Agro Activity
* DELETE
* path: ```/api/agro-activities/{agroActivityId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE


<img width="400" alt="Zrzut ekranu 2024-11-8 o 18 30 50" src="https://github.com/user-attachments/assets/33fb9eeb-70ae-42cb-b56c-107f7efaa81d">


# 5. Get all tasks for logged user
* GET
* path: ```/api/agro-activities/assigned```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER``` or ```ROLE_FARM_EQUIPMENT_OPERATOR```
* Example body: NONE
* Request param: NONE


<img width="400" alt="Zrzut ekranu 2024-11-18 o 21 46 41" src="https://github.com/user-attachments/assets/f22999f7-3254-438a-a11e-43751b107b55">

# 6. Mark task as completed
* PATCH
* path: ```/api/agro-activities/complete/{activityId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER``` or ```ROLE_FARM_EQUIPMENT_OPERATOR```
* Example body: NONE

<img width="400" alt="Zrzut ekranu 2024-11-18 o 21 46 33" src="https://github.com/user-attachments/assets/59f99d91-390e-4f8e-a95b-e4c9a911d65d">


# 7. Get all activity category names
* GET
* path: ```/api/agro-activities/available-category```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE
* Request param: NONE

<img width="400" alt="Zrzut ekranu 2024-11-8 o 18 30 59" src="https://github.com/user-attachments/assets/100a5064-3bac-405b-ae19-86a287658f01">



