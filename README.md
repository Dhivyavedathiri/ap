// Import Axios in a Node.js environment or include it in your HTML file for browsers
const axios = require('axios');

// Define the object you want to send
const dataObject = {
  key1: 'value1',
  key2: 'value2',
  // Add other properties as needed
};

// Define the API endpoint (replace 'your-api-endpoint' with the actual endpoint)
const apiEndpoint = 'https://crudcrud.com/api/your-api-endpoint';

// Make a POST request
axios.post(apiEndpoint, dataObject)
  .then(response => {
    console.log('POST Request Successful:', response.data);
  })
  .catch(error => {
    console.error('Error:', error);
  });
