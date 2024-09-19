# 1. Signup new Farm with farm manager
* POST
* path: ```/api/auth/signupfarm ```
* Required role: NONE
* Example body:

``` json
{
	"firstName": "Mieczysław",
	"lastName": "Nowak",
	"username": "Operator9",
	"email": "test9@test.pl",
	"password": "123456",
	"phoneNumber": "697122472",
	"farmName": "Zielone pola",
	"activationCode": "0y4U1SaR"
}
```
<img width="400" alt="Zrzut ekranu 2024-09-9 o 17 35 29" src="https://github.com/user-attachments/assets/3ac7b4da-ae6a-4707-a94a-ffdd93a776af">


# 2. Signup new user
* POST
* path: ```/api/auth/signup```
*  Required role: ```ROLE_FARM_MANAGER``` or ```ROLE_FARM_OWNER```
* Example body:

``` json
{
	"firstName": "Mieczysław",
	"lastName": "Nowak",
	"username": "Operator7",
	"email": "test7@test.pl",
	"role": "ROLE_FARM_MANAGER",
	"password": "123456",
	"phoneNumber": "697122470"
}
```

<img width="400" alt="Zrzut ekranu 2024-09-4 o 21 07 25" src="https://github.com/user-attachments/assets/67c288b5-8f89-4fbf-b658-3f102e9e0017">
 


# 3.Signin any user
* POST
* path: ```/api/auth/signin```
* Required role: NONE
* Example body:

``` json
{
	"username": "Operator7",
	"password": "123456"
}
```

<img width="400" alt="Zrzut ekranu 2024-09-18 o 23 03 52" src="https://github.com/user-attachments/assets/275debab-cab6-4968-86aa-24c18356a51d">



# 4.Signout any user
* POST
* path: ```/api/auth/signout```
* Required role: NONE
* Example body: NONE

<img width="400" alt="Zrzut ekranu 2024-09-4 o 21 43 16" src="https://github.com/user-attachments/assets/1481c26e-7aeb-4d8e-bef5-4c0ecf4cd0d7">
