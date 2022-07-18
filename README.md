**Laravel JWT auth server**
*

## [POST] /api/auth/register

    {
    	"name":"username",
    	"email":"useremail@gmail.com",
    	"password":"pwd"
    }
## [POST] /api/auth/login

    { 
    	"email":"useremail@gmail.com",
    	"password":"pwd"
    }
## Two way to send token 

    {
    	"Authorization":"Bearer <jwt_token>"
    }
    
	/api/me?token=<JWT_TOKEN>
## [POST] /api/auth/me?token=<jwt_token>

    { 
    	"email":"useremail@gmail.com",
    	"password":"pwd"
    }
## [POST] /api/auth/me 

	 //headers
	 {
    	"Authorization":"Bearer <jwt_token>"
	 }
	 //request body 
     { 
    	"email":"useremail@gmail.com",
    	"password":"pwd"
     }
## [POST] /api/auth/refresh?token=<jwt_token>
## [POST] /api/auth/refresh

	 //headers
	 {
    	"Authorization":"Bearer <jwt_token>"
	 } 

## [POST] /api/auth/logout?token=<jwt_token>
## [POST] /api/auth/logout

	 //headers
	 {
    	"Authorization":"Bearer <jwt_token>"
	 } 


