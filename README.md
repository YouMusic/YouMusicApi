**YouMusic API Description**
----
  <_Dies ist der API-Call welcher von den Benutzern benutzt wird um die Audiospur eines Videos zu streamen._>

* **/stream/get/videoid**

  <_The URL Structure (path only, no root url)_>

* **Method:**
  
  <_The request type_>

  `GET`

* **Success Response:**
  
  <_What should the status code be on success and is there any returned data? This is useful when people need to to know what their callbacks should expect!_>

  * **Code:** 200 <br />
    **Content:** `{ streaming-url : https://examplestream.com/exampleid }`
 
* **Error Response:**

  <_Most endpoints will have many ways they can fail. From unauthorized access, to wrongful parameters etc. All of those should be liste d here. It might seem repetitive, but it helps prevent assumptions from being made where they should be._>

  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "Log in" }`

  OR

  * **Code:** 429 UNPROCESSABLE ENTRY <br />
    **Content:** `{ error : "To many requests" }`

* **Sample Call:**

  <_This is a sample curl call to this API._> 

* **Notes:**

  <_This is where all uncertainties, commentary, discussion etc. can go. I recommend timestamping and identifying oneself when leaving comments here._> 
