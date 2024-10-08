# 1. GET landparcels list
* GET
* path: ```/api/landparcel/all```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE
* Request param:
  - Optional String: ```searchString```
  - Optional Double: ```minArea```
  - Optional Double: ```maxArea```
 

<img width="400" alt="Zrzut ekranu 2024-10-8 o 19 40 14" src="https://github.com/user-attachments/assets/88483787-c22b-4c35-b405-23b8fe4f55e1">


# 2. GET landparcel details
* GET
* path: ```/api/landparcel/{id}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE
* Request param: NONE

<img width="400" alt="Zrzut ekranu 2024-10-8 o 19 56 35" src="https://github.com/user-attachments/assets/760e93b0-d817-48b9-a77e-96e15beb14d5">

# 3. Add landparcel
* POST
* path: ```/api/landparcel/new```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: 
```json
{
    "landOwnershipStatus": "STATUS_PRIVATELY_OWNED",
    "voivodeship": "świętokrzyskie",
    "district": "Rzeszowskie",
    "commune": "Dęblin",
    "geodesyRegistrationDistrictNumber": "488",
    "landparcelNumber": "2593/4",
    "longitude": 23.9973,
    "latitude": 49.6309,
    "area": 13.53
}
```

<img width="400" alt="Zrzut ekranu 2024-10-8 o 19 59 20" src="https://github.com/user-attachments/assets/de507573-faa9-4bd2-89b6-6c0b4157e9b1">

# 4. Update landparcel
* PUT
* path: ```/api/landparcel/{id}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body:

```json
{
    "landOwnershipStatus": "STATUS_PRIVATELY_OWNED",
    "longitude": 23.9973,
    "latitude": 49.6309,
    "area": 10.53
}
```
* Description:
- In the case of update data, it is only allowed for the above parameters

<img width="400" alt="Zrzut ekranu 2024-10-8 o 20 01 05" src="https://github.com/user-attachments/assets/1c32c523-8966-4b1e-8100-2e0f0d0bb06a">

# 4. Delete landparcel
* DELETE
* path: ```/api/landparcel/{id}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```ROLE_FARM_MANAGER```
* Example body: NONE

<img width="400" alt="Zrzut ekranu 2024-10-8 o 20 03 58" src="https://github.com/user-attachments/assets/7b1670a9-f1dc-4cea-a954-53740e891e49">




