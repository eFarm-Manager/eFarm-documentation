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
* Params: NONE

<img width="400" alt="Zrzut ekranu 2024-11-7 o 13 43 34" src="https://github.com/user-attachments/assets/497a8a29-3889-4e8e-8958-2d7ac465b8c0">


# 3. Get Agro Activity details
* GET
* path: ```/api/agro-activities/details/{agroActivityId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE
* Params: NONE


<img width="400" alt="Zrzut ekranu 2024-11-7 o 13 45 44" src="https://github.com/user-attachments/assets/f72c694f-3cb6-4dae-a13c-c1542b59127b">

