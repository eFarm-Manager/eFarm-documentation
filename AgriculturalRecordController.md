# 1. GET all records per season
* GET
* path: ```/api/records/all```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"``` or ```"ROLE_FARM_EQUIPMENT_OPERATOR"```
* Example body: NONE
* Optional parameters:
  - season
  - searchQuery



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

# 3. Update agriculture record
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

# 4. Get available seasons
* GET
* path: ```/api/records/available-seasons```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE


# 5. Get available crops
* GET
* path: ```/api/records/available-crops```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE


