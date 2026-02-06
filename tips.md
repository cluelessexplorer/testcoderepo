# Aparna's tips and handy references

## CURL

### OPTIONS
curl -v -X OPTIONS "https://api.example.com/v1/resources" \
  -H "Origin: https://app.example.com" \
  -H "Access-Control-Request-Method: POST" \
  -H "Access-Control-Request-Headers: Authorization, Content-Type"

curl -v -X OPTIONS "https://api.example.com/v1/resources" \
  -H "Origin: https://app.example.com" \
  -H "Access-Control-Request-Method: GET" \
  -H "Access-Control-Request-Headers: Authorization"


### GET
curl -v -X GET "https://api.example.com/v1/profile" \
  -H "Authorization: Bearer <ACCESS_TOKEN>" \
  -H "Accept: application/json"

curl -v -u username:password \
  https://api.example.com/v1/resources

### POST (json)
curl -v -X POST "https://api.example.com/v1/resources" \
  -H "Content-Type: application/json" \
  -H "Accept: application/json" \
  -d '{
        "name": "Sample",
        "status": "ACTIVE"
      }'

### POST (x-www-form-urlencoded)
curl -v -X POST "https://auth.example.com/oauth/token" \
  -H "Content-Type: application/x-www-form-urlencoded" \
  -d "grant_type=authorization_code" \
  -d "client_id=client123" \
  -d "client_secret=secret456" \
  -d "code=AUTH_CODE"

### POST (multipart/form-data)
curl -v -X POST "https://api.example.com/v1/upload" \
  -H "Authorization: Bearer <ACCESS_TOKEN>" \
  -F "file=@document.pdf" \
  -F "metadata={\"type\":\"invoice\"};type=application/json"



### PUT
curl -v -X PUT "https://api.example.com/v1/resources/123" \
  -H "Content-Type: application/json" \
  -d '{
        "name": "Updated Name",
        "status": "INACTIVE"
      }'


### PATCH
curl -v -X PATCH "https://api.example.com/v1/resources/123" \
  -H "Content-Type: application/json" \
  -d '{
        "status": "ACTIVE"
      }'

## MAC
To zip folder
Go to Terminal
Go to the parent of <folder_to_be_zipped>
zip -r zipFile.zip <folder_to_be_zipped>

## LINUX

## JavaScript

## Python
