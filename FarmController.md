# 1. GET all farm users
* GET
* path: ```/api/farm/users```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE


<img width="400" alt="Zrzut ekranu 2024-09-18 o 12 21 36" src="https://github.com/user-attachments/assets/77825c18-2201-4819-ac15-71dac9bc5851">


# 2. GET farm details
* GET
* path: ```/api/farm/details```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE

  <img width="400" alt="Zrzut ekranu 2024-09-25 o 23 01 53" src="https://github.com/user-attachments/assets/ef76075a-75fe-4f08-ae8a-95eab60bdfc1">

* Description:
   - if user has Role "ROLE_FARM_OWNER" then have all info about farm (with expireCodeDate)
   - if user has Role "ROLE_FARM_MANAGER" then have information with expireCodeDate set as null
 
# 3. UPDATE farm details
* PUT
* path: ```/api/farm/details```
* Required role: ```"ROLE_FARM_OWNER"```
* Example body:
``` json
{
    "farmName": "Zielone sady południa",
    "farmNumber": "123456",
    "zipCode": "22-400"
}
```
<img width="400" alt="Zrzut ekranu 2024-09-25 o 23 01 53" src="https://github.com/user-attachments/assets/41962e0f-f88f-4104-b9e9-821fcb5f8614">



