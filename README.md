# CS-361-Project
const express = require('express');
const app = express();

// Define endpoint for supplements request
app.get('/supplements', (req, res) => {
  // Retrieve data on 5 exercise supplements
  const supplements = getExerciseSupplements();
  // Return supplements data as response
  res.json(supplements);
});

// Function to retrieve data on 5 exercise supplements
function getExerciseSupplements() {
  // Connect to database or external API to retrieve supplement data
  // Query database or API to retrieve data on 5 supplements
  const supplementData = [
    { name: 'Whey Protein', description: 'A fast-absorbing protein supplement that helps support muscle growth and recovery.' },
    { name: 'Creatine', description: 'A supplement that helps increase energy and power during high-intensity exercise.' },
    { name: 'BCAAs', description: 'Amino acids that help support muscle recovery and reduce muscle soreness.' },
    { name: 'Pre-Workout', description: 'A supplement that contains caffeine and other ingredients to help increase energy and focus during exercise.' },
    { name: 'Fish Oil', description: 'A supplement that contains omega-3 fatty acids to help reduce inflammation and support overall health.' }
  ];
  return supplementData;
}

// Start the server
app.listen(3000, () => console.log('Server listening on port 3000'));
