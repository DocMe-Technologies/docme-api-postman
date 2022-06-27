# docme-api-postman
#### API calls for vital stats

## Import API
- Install Postman
- File -> Import -> DocMeAPI.postman_collection.json

## Run API Calls
- POST Upload Video
	- Headers:
		- X-Token: change if provided or leave the default value
	- Body
		- video: upload any video, preferably a 20 second portrait video
	- Response( after sending the call ):
		- id: copy value for using it to access the processed data in GET API call
- GET Get Status
	- Link:
		- Paste the id provided by the POST response after v1/measurement/
		- the default link gets the vitals of an old video upload
	- Headers:
		- X-Token: change if provided or leave the default value

