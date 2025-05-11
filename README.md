//Register request ![img.png](img.png)
curl --location --request POST 'localhost:8080/api/auth/register' \
--header 'Content-Type: application/json' \
--data-raw '{
"username": "satish-ahirwar",
"email": "satishlariya@gmail.com",
"password": "TechMy@",
"role": [
"admin"
]
}'

// Login Request
curl --location --request POST 'localhost:8080/api/auth/login' \
--header 'Content-Type: application/json' \
--header 'Cookie: tech-access-token=eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJzYXRpc2gtYWhpcndhciIsImlhdCI6MTc0Njk2ODc5NCwiZXhwIjoxNzQ2OTY4ODU0fQ.186_3s8Ob4T0MtlTQq4vLAks9QR0AxpgIww3j35oEJA' \
--data-raw '{
"username": "satish-ahirwar",
"password": "TechMy@"
}'

