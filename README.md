![Header Image](https://github.com/logananthony/arm-angles-statcast/blob/main/Arm%20Angles.png)

# Calculating Arm Angles Using Statcast Data

## Introduction
This [project](https://github.com/logananthony/arm-angles-statcast/blob/main/Calculating%20Arm%20Angles%20Using%20Statcast%20Data%20%7C%20Rundown%20Baseball.pdf) aims to calculate the arm angles of pitchers using Statcast data in R. The motivation for this project originated from the 2020 ALCS, where the diversity in release points of the Rays pitching staff highlighted the importance of understanding arm angles. Arm angles offer a more interpretable version of release points, providing valuable insights for both mechanical and analytical purposes in baseball.

## Research Questions
The primary motivation behind calculating arm angles is to enhance our understanding of pitchers' mechanics and their impact on performance. Here are some key questions that this project seeks to address:
- How are arm angles distributed among pitchers?
- Do bullpens with a high variance in arm angles perform better?
- What is the relationship of arm angles between pitches?
- Do pitchers with dramatically different arm angles between pitches perform statistically worse?
- How accurately can spin axes be calculated from arm angle?
- How can we understand pitchers who purposely change arm angles, like Rich Hill or Nestor Cortes, better?
- Do pitchers with certain arm slots throw pitch X or pitch Y better than pitchers without that arm slot?
- Can we use arm angles to better classify pitchers using cluster algorithms?
- How do arm angles change with age?
- How can arm angle consistency be defined?

## Calculation Method
The calculation of arm angles involves forming triangles using the release position metrics provided by Statcast. The key steps include:
1. **Defining the Axes**: The Y-axis works vertically from home plate to center field, and the X-axis measures horizontal distance east to west. The Z-axis measures height.
2. **Forming Triangles**: Using the average release positions, a triangle is formed where the hypotenuse represents the pitcher's arm.
3. **Calculating Angles**: By using trigonometric equations, the arm angle (θ) is calculated in radians and then converted to degrees.


## Getting Started
To get started with this project, follow these steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/logananthonymlb/arm-angles-statcast.git
    cd arm-angles-statcast
    ```

2. **Install Dependencies**:
    ```r
    install.packages(c("tidyverse", "ggplot2"))
    ```

3. **Run the Calculations**:
    Open `arm-angles.Rmd` in RStudio and knit the document to produce the results.

## Contributing
Contributions are welcome! If you have any suggestions or improvements, please fork the repository and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

