# docme-api-postman
#### API calls for vital stats

## Import API
- Install Postman
- File -> Import -> DocMeAPI.postman_collection.json

## Run API Calls
- Video example:
	- https://github.com/DocMe-Technologies/docme-api-postman/blob/main/Screen%20Recording%202022-06-27%20at%2013.45.26.mov
- POST Upload Video
	- Headers:
		- X-Token: change if provided or leave the default value
	- Body
		- video: upload any video, preferably a 20 second portrait video
	- Response( after sending the call ):
		- id: copy value for using it to access the processed data in GET API call
<img width="855" alt="Screenshot 2022-06-23 at 17 11 18" src="https://user-images.githubusercontent.com/106098821/175922904-311c31cf-e423-4026-8547-384cc28e48e6.png">

- GET Get Status
	- Link:
		- Paste the id provided by the POST response after v1/measurement/
		- the default link gets the vitals of an old video upload
	- Headers:
		- X-Token: change if provided or leave the default value

<img width="855" alt="Screenshot 2022-06-23 at 17 13 21" src="https://user-images.githubusercontent.com/106098821/175922973-42997562-7081-4ebb-9dfc-1004568921cb.png">
