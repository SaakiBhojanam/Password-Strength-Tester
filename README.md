# Password Strength Checker

## Overview

This project is a **Password Strength Checker** web application designed to evaluate the strength of a user's password in real-time. It categorizes the password as "Weak," "Medium," or "Strong" based on specific criteria such as length, the inclusion of numbers, special characters, and mixed case letters.

## Features

- **Real-Time Feedback**: As the user types, the strength of the password is dynamically assessed and displayed.
- **Clear Criteria**: Provides a breakdown of what makes a password weak, medium, or strong.
- **Responsive Design**: Works seamlessly on different screen sizes.

## Criteria for Password Strength

1. **Weak**: Less than 8 characters.
2. **Medium**: At least 8 characters with a mix of letters and numbers.
3. **Strong**: At least 10 characters with letters, numbers, and special characters.

## How It Works

1. **Input Field**: Users enter their password in the input box.
2. **Password Evaluation**: 
   - The script checks the password's length.
   - It scans for numbers, special characters, and mixed-case letters.
3. **Dynamic Feedback**: The password strength is displayed as one of the following:
   - **Weak**: Displayed in red.
   - **Medium**: Displayed in orange.
   - **Strong**: Displayed in green.

## Technology Stack

- **HTML**: For the structure of the webpage.
- **CSS**: For styling the application, ensuring a clean and professional look.
- **JavaScript**: For dynamically evaluating the password strength and updating the UI in real time.

### Example: Adjusting Criteria
To change the criteria for "Strong" passwords, update the `getPasswordStrength` function:
```javascript
if (password.length >= 12 && hasNumbers && hasSpecialChars && hasMixedCase) {
  return 'strong';
}
