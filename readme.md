### Making requests

The user must be logged in at https://ux.nineweb.co.th/accounts/login/ to obtain the auth cookies `csrftoken` and `sessionid`. For the AJAX request, the cookies `csrftoken` and `sessionid` must be sent with each request. 

ex ```curl -b "csrftoken=alwLKweCOSDKekSODFLKWERo" -b "sessionid=7wslksf2324s5g" https://ux.nineweb.co.th/api/test/```

### Tests endpoint

**To get list of tests:**  
`https://ux.nineweb.co.th/api/test/`

 *question types:*

S : Single Answer

T : Text
  

**To get list of questions for test:**  
`https://ux.nineweb.co.th/api/test/<test ID>`  
**question_set** are the test questions.
see test.json for example payload  

**To submit form data:**  
PUT request to 
`https://ux.nineweb.co.th/api/test/<test ID>/`  
see result.json for example payload