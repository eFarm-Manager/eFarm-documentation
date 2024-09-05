1. Signup new user
* POST
* path: /api/auth/signin
* Example body:
{
	"firstName": "Mieczysław",
    "lastName": "Nowak",
    "username": "Operator7",
    "email": "test7@test.pl",
    "role": "ROLE_FARM_MANAGER",
    "password": "123456",
    "phoneNumber": "697122470"
}

<img width="849" alt="Zrzut ekranu 2024-09-4 o 21 07 25" src="https://github.com/user-attachments/assets/67c288b5-8f89-4fbf-b658-3f102e9e0017">


2.Signin any user
* POST
* path: /api/auth/signin
* Example body:
{
	"username": "Operator7",
    "password": "123456"
}

<img width="846" alt="Zrzut ekranu 2024-09-4 o 21 13 06" src="https://github.com/user-attachments/assets/d8d94b06-4f56-480a-90b6-4df4e71a0b72">


3.Singout any user
* POST
* path: /api/auth/signout
* Example body: NONE

<img width="849" alt="Zrzut ekranu 2024-09-4 o 21 43 16" src="https://github.com/user-attachments/assets/1481c26e-7aeb-4d8e-bef5-4c0ecf4cd0d7">
