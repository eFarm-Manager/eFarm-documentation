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

<img width="400" alt="Zrzut ekranu 2024-11-5 o 20 57 25" src="https://github.com/user-attachments/assets/1b69096b-b11e-4569-ade5-55886872f7c2">


Obecnie:

![Screenshot from 2024-11-05 21-27-12](https://github.com/user-attachments/assets/6c8f9ddc-f4d6-4bd6-988a-eb543d9008e0)
