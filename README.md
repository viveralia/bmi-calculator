# BMI Calculator
Body mass index (BMI) is a measure of body fat based on height and weight that applies to adult men and women.

![Formula](https://i.ibb.co/YtGVpvb/Captura-de-Pantalla-2020-05-12-a-la-s-9-37-03-p-m.png)

## Instructions
### Iteration 1 | Create the components
You will create the following components:
- `HeightInput`
- `WeightInput`
- `Result`

The `App` component must serve as a Layout for storing all the states and communicating with its children via props. [It should look something like this](https://www.nhlbi.nih.gov/health/educational/lose_wt/BMI/bmi-m.htm):

``` jsx
import React from 'react'

const App = () => {
  return (
    <div>
      <HeightInput />
      <WeightInput />
      <button>Calculate my BMI<button>
      <Result />
    </div>
  )
}
```

### Iteration 2 | Calculation
When the user fills both fields and presses the button, the app should calculate his BMI and show the corresponding status:
- Underweight *(less than 18.5)*
- Normal weight *(18.5 – 24.9)*
- Overweight *(25 – 29.9)*
- Obesity *(30 or more)*

Beware that the inputs require the following **validations**:
- Both fields are required
- Both fields must be numbers
- Min height is 1m and max height is 3m
- Min weight is 1kg and max weight is 200kg

### Bonus
Pimp the app with some styles. Choose one of the following:
- Styled components with emotion
- CSS modules
- Material UI or Ant Design
- Bulma

Remember to give it the styles with **mobile-first mindset**. The app must look gorgeous on mobile, tablet and desktop.

Happy coding! ❤️