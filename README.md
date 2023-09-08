# random_image_gnerator

# Logic => btn, carContainer, carImg, carName: These variables are used to select HTML elements on the page using JavaScript. btn.addEventListener("click", ...): This listens for a click event on a button with the ID "btn".

When the button is clicked, the function inside the event listener is executed

It starts by setting the src attribute of carImg (which likely represents an image element) to "spinner.svg". This probably shows a loading spinner while waiting for the API response.
It then sends a request to the Unsplash API using fetch(). The URL for the request points to a random car image with a specific query parameter and an access key.
After fetching the data, it parses the response as JSON and assigns it to the data variable. It updates the button text to "Get Cars".
It sets the display style property of carContainer to "block" to make it visible. It updates the src attribute of carImg to the URL of the random car image received from the API.
It updates the text content of carName with the "alt_description" of the image received from the API.

If there's an error during the API request (e.g., no internet connection or API server is down), it catches the error.
It logs the error to the console. It re-enables the button if it was disabled. It sets the button text back to "Get car". It updates the text content of carName to indicate that an error occurred.
