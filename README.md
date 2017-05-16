**YouMusic API Description**
----
  Dies ist der API-Call welcher von den Benutzern benutzt wird um die Audiospur eines Videos zu streamen.

* **/stream/get/_videoid_**

* **Method:**
  
  The request type

  `GET`

* **Success Response:**
  
  * **Code:** 200 <br />
    **Content:** `{ streaming-url : https://examplestream.com/exampleid }`
 
* **Error Response:**

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "Log in" }`

  OR

  * **Code:** 429 UNPROCESSABLE ENTRY <br />
    **Content:** `{ error : "To many requests" }`

* **Sample Call:**

  This is a sample curl call to this API.
