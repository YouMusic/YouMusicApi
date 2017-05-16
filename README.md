**YouMusic API Beschreibung**
----
  This is the API call which is used to stream the audio data of a video from youtube.

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

  This is a example cURL call to our API which stores the returned data in a file named _response.json_
  
  ```
  curl http://youmusic.com/api/v1/stream/2gFJuEbk5DY > response.json
  ```
