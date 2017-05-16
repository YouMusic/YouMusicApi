**YouMusic API Description**
----
  Dies ist der API-Call welcher benutzt wird um die Audiospur eines Videos zu streamen.

* **/stream/_videoid_**

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

  Dies ist ein simpler, cURL call auf unsere API, welcher die empfangenen daten in ein file namens response.json speichert.
  
  ```
  curl http://youmusic.com/api/v1/stream/2gFJuEbk5DY 1> response.json
  ```
