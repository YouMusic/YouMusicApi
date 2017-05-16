**YouMusic API Description**
----
  Dies ist der API-Call welcher benutzt wird um die Audiospur eines Videos zu streamen.

* **/stream/get/_videoid_**

* **Method:**

  `GET`

* **Success Response:**
  
  * **Code:** 200 <br />
    **Content:** `{ streaming-url : https://examplestream.com/exampleid }`
 
* **Error Response:**

  * **Code:** 429 TO MANY REQUESTS <br />
    **Content:** `{ error : "To many requests" }`

  OR

  * **Code:** 422 UNPROCESSABLE ENTRY <br />
    **Content:** `{ error : "Unprocessable entry" }`

* **Sample Call:**

  This is a sample curl call to this API.
