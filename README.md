Setup Instructions

Install XAMPP if you haven't already.
Copy the entire my_api_gateway/ folder into your htdocs/ directory (e.g., C:\xampp\htdocs\my_api_gateway).
Start Apache and MySQL from the XAMPP Control Panel.
Create a MySQL database use the apigatewaydb.sql Copy and Paste it.

Valid API Keys Implemented imag

How to test features (POSTMAN/ CURL) Remember: You must always include the header X-API-Key when making requests.

Accessing /users Service. •Method: GET •URL: http://localhost:8080/my_api_gateway/api/users •Headers: •X-API-Key: key123 •X-API-Key: key456 
![image](https://github.com/user-attachments/assets/52fb68d9-99c6-4b67-a6fa-f5ba15f3940c)


Accessing /products Service. •Method: GET •URL: http://localhost:8080/my_api_gateway/api/products •Headers: •X-API-Key: key123 •X-API-Key: key456 
![image](https://github.com/user-attachments/assets/c13ebc0a-ad7c-4545-8bcd-d78b23ba6c54)


Accessing /dashboard Service. •Method: GET •URL: http://localhost:8080/my_api_gateway/api/dashboard •Headers: •X-API-Key: key123 •X-API-Key: key456 
![image](https://github.com/user-attachments/assets/9a32b512-d94c-4d1d-9fed-ba169a0c5331)


Challenges Faced / Assumptions Made 
Challenge: 
Testing with Postman and curl
Properly simulating real-world requests required adding headers manually in Postman or crafting curl commands. Without these headers (like X-API-Key), the gateway would reject requests, which initially led to confusion during testing.


Assumption: 
API Key Transmission via X-API-Key Header
It was assumed clients would consistently send the API key via the X-API-Key custom HTTP header for authentication, and this header would be supported by tools like Postman and curl.

Unauthorized User: 
![image](https://github.com/user-attachments/assets/9dfde1a9-c9b8-4167-bde3-cfb40ea55580)


Rate Limiter: 
![image](https://github.com/user-attachments/assets/626e0ecb-367c-448f-a0db-85fcd89f5f26)



Gateway Logs: 
![image](https://github.com/user-attachments/assets/29eff3de-875b-450a-bb83-efe63c269eae)



