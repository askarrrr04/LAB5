# LAB5
function calculateBMI(weight, height) {
  // Convert height to meters
  height = height / 100;

  // Calculate BMI
  const bmi = weight / (height * height);

  return bmi.toFixed(2);
}

function getBMIStatus(bmi) {
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
