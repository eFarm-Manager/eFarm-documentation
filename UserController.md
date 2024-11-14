# 1. GET all farm users
* GET
* path: ```/api/users/all```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE
* Request params: NONE


<img width="400" alt="Zrzut ekranu 2024-11-8 o 20 37 38" src="https://github.com/user-attachments/assets/ec0c4ecc-c754-4bc3-942e-a6bedd096bf0">

# 2. GET Active farm Users
* GET
* path: ```/api/users/active```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE
* Request params: NONE

<img width="400" alt="Zrzut ekranu 2024-11-8 o 20 37 47" src="https://github.com/user-attachments/assets/5669468f-ee60-44ab-8042-0c707debe1b8">

# 3. Update user properties
* PUT
* path: ```/api/users/update/{userId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body:

```json
{
    "firstName": "Jan",
    "lastName": "Kowalski",
    "email": "jan.kowalski@example.com",
    "phoneNumber": "+48123456789",
    "role": "ROLE_FARM_MANAGER"
}
```
<img width="400" alt="Zrzut ekranu 2024-11-14 o 18 31 45" src="https://github.com/user-attachments/assets/cf2f638e-b7aa-4da7-8e36-80dcd66bdda3">

# 4. Toggle user active status
* PATCH
* path: ```/api/users/toggle-active/{userId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE
* Request params: NONE

<img width="400" alt="Zrzut ekranu 2024-11-14 o 18 31 29" src="https://github.com/user-attachments/assets/8a05804c-bcb8-428f-8686-46f4a4cf7c63">

# 5 Change user password by farm manager
* PUT
* path: ```/api/users/update-password/{userId}```
* Required role: ```"ROLE_FARM_OWNER"``` or ```"ROLE_FARM_MANAGER"```
* Example body: NONE
* Request params: NONE


<img width="400" alt="Zrzut ekranu 2024-11-14 o 18 31 52" src="https://github.com/user-attachments/assets/022670a8-db21-4a43-bf83-7d315f2af7d6">
