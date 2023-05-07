# CS-361-Project
In order to receive and use the data from the microservice, the steps below are required.
Make sure you have Node.js installed on your machine. If you don't have it installed, you can download it from the official website: https://nodejs.org/en/download/
Copy the code for the microservice into a file, and save it with a .js extension (e.g. supplements.js).
Open a command prompt or terminal window in the directory where you saved the file.
Install the required packages by running the following command: npm install express
Start the microservice by running the following command: node supplements.js
Open a web browser and navigate to http://localhost:3000/supplements. This sends a GET request to the /supplements endpoint, which triggers the getExerciseSupplements() function to retrieve the data on five exercise supplements, and return it as a JSON object.
You should see the data on the five exercise supplements displayed in your web browser as a JSON object.
