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

* Description:
   - if days to expiration <= 14 then we have massage ```expireCodeInfo```, which should be shown on frontend (in the other situations it is ```null```)
   - if activationCode expired then we have http status 403 and info about expired code, then should be use ```location``` parameter to redirect on frontend to ```/api/auth/update-activation-code```

<img width="400" alt="Zrzut ekranu 2024-09-18 o 23 03 52" src="https://github.com/user-attachments/assets/275debab-cab6-4968-86aa-24c18356a51d">
     
  ![Zrzut ekranu 2024-09-19 o 20 32 19](https://github.com/user-attachments/assets/a0052e45-87c7-4afd-b6db-cf7c88a82aa0)

# 4.Update activation code
* POST
* path: ```/api/auth/update-activation-code```
* Required role: ROLE_FARM_OWNER
* Example body: 

``` json
{
	"username": "Operator7",
	"password": "123456",
	"newActivationCode": "G4Yu78jh"
}
```
* Description:
	- if the code update was successful, you should be redirected to the login page using the "location" parameter

![Zrzut ekranu 2024-09-19 o 20 21 49](https://github.com/user-attachments/assets/25d94a6e-c9d7-4a31-acc4-cab99beadb20)

![Zrzut ekranu 2024-09-19 o 20 31 20](https://github.com/user-attachments/assets/f1142aa3-3019-4acd-a6cc-ce32a5e02f17)


# 5.Signout any user
* POST
* path: ```/api/auth/signout```
* Required role: NONE
* Example body: NONE

<img width="400" alt="Zrzut ekranu 2024-09-4 o 21 43 16" src="https://github.com/user-attachments/assets/1481c26e-7aeb-4d8e-bef5-4c0ecf4cd0d7">

