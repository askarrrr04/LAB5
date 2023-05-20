# LAB5
function calculateBMI(weight, height) {
  // Convert height to meters
  height = height / 100;

  // Calculate BMI
  const bmi = weight / (height * height);

  return bmi.toFixed(2);
}

<<<<<<< HEAD
function getBMIStatus1(bmi) {
=======
function getBMI(bmi) {
>>>>>>> bdbf3302bc7beaafd1abd780eb05b727f5ce459d
  if (bmi < 18.5) {
    return "Your BMI is " + bmi + ", which means you are underweight.";
  } else if (bmi >= 18.5 && bmi <= 24.9) {
    return "Your BMI is " + bmi + ", which means you have a normal weight.";
  } else {
    return "Your BMI is " + bmi + ", which means you might be overweight.";
  }
}

// Example usage:
const weight = 70; // in kilograms
const height = 170; // in centimeters

const bmi = calculateBMI(weight, height);
const bmiStatus = getBMIStatus(bmi);

bmiStatus;
