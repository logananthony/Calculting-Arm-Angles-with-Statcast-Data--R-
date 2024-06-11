![Header Image](https://github.com/logananthony/arm-angles-statcast/blob/main/Arm%20Angles.png)

# Calculating Arm Angles Using Statcast Data

## Introduction
From an [old](https://github.com/logananthony/arm-angles-statcast/blob/main/Calculating%20Arm%20Angles%20Using%20Statcast%20Data%20%7C%20Rundown%20Baseball.pdf) article of mine but I found the moitivation to ressurect it from a thread on Twitter/X from Trevor Thrash who has created his own calculations in [python](https://github.com/trevorwthrash/armAngles) - check it out. Anyway, this project aims to calculate the arm angles of pitchers using Statcast data in R. The motivation for this project originated from the 2020 ALCS, where the diversity in release points of the Rays pitching staff was highlighted in a [graph](https://github.com/logananthony/arm-angles-statcast/blob/main/2020%20Rays%20Graph.jpg) during one of the games. This was the primary motivation behind calculating arm angles; the pursuit to further enhance our understanding of pitchers' mechanics and their impact on performance. Of course this is just a method of approximation, we could very likely get the accurate measurments of this as time goes on so take it for what it's worth.

## Calculation Method
The calculation of arm angles involves forming triangles using the release position metrics provided by Statcast. The key steps include:
1. **Defining the Axes**: The Y-axis works vertically from home plate to center field, and the X-axis measures horizontal distance east to west. The Z-axis measures height.
2. **Forming Triangles**: Using the average release positions, a triangle is formed where the hypotenuse represents the pitcher's arm.
3. **Calculating Angles**: By using trigonometric equations, the arm angle (θ) is calculated in radians and then converted to degrees.


## Getting Started
To get started with this project, follow these steps (I should also note I didn't incldue any packages to retrieve the statcast data but [baseballr](https://billpetti.github.io/baseballr/) is a great one for R or if you prefer python [pybaseball](https://github.com/jldbc/pybaseball) is equally fantastic!):

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

