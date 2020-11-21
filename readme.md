### Making requests

The user must be logged in at https://ux.nineweb.co.th/accounts/login/ to obtain the cookie `csrftoken`. For the AJAX request, the header of `X-CSRFToken` with the token must be sent with each request.

### Tests endpoint

**To get list of tests:**  
`https://ux.nineweb.co.th/api/test/`  

**To get list of questions for test:**  
`https://ux.nineweb.co.th/api/test/<test ID>`  
**question_set** are the test questions.
see test.json for example payload  

**To submit form data:**  
PUT request to 
`https://ux.nineweb.co.th/api/test/<test ID>/`  
see result.json for example payload