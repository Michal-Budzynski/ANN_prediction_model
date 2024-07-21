# Power Plant Energy Output Prediction Model

This project aims to predict the electrical energy output of a Combined Cycle Power Plant using a machine learning model (Artificial Neural Networks). The prediction is based on various environmental and operational factors.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Project Structure](#project-structure)
3. [Data Description](#data-description)
4. [Evaluation](#evaluation)
5. [Contributing](#contributing)
6. [License](#license)

## Project Overview
Combined Cycle Power Plants (CCPP) generate electricity by combining gas and steam turbines. This project uses a Artificial Neural Networks techinque to predict the power output (`PE`) based on various environmental variables such as temperature (`AT`), ambient pressure (`AP`), and relative humidity (`RH`).

## Project Structure
The project consists of the following files:
- `code.ipynb`: Jupyter notebook containing the code for data analysis, model training, and evaluation.
- `data.xlsx`: Excel file containing the dataset used for training and testing the model.
  
## Data Description
The dataset used in this project consists of the following columns:
- `AT` (Temperature in °C): The ambient temperature.
- `V` (Exhaust Vacuum): The exhaust vacuum.
- `AP` (Ambient Pressure in mbar): The ambient pressure.
- `RH` (Relative Humidity in %): The relative humidity.
- `PE` (Energy Output in MW): The net hourly electrical energy output.

Here is a preview of the data:

| AT    | V     | AP     | RH    | PE     |
|-------|-------|--------|-------|--------|
| 14.96 | 41.76 | 1024.07| 73.17 | 463.26 |
| 25.18 | 62.96 | 1020.04| 59.08 | 444.37 |
|  5.11 | 39.40 | 1012.16| 92.14 | 488.56 |
| 20.86 | 57.32 | 1010.24| 76.64 | 446.48 |
| 10.82 | 37.50 | 1009.23| 96.62 | 473.90 |

## Evaluation
The performance of the model is evaluated using two metrics: Mean Absolute Percentage Error (MAPE) and Root Mean Squared Percentage Error (RMSPE).

- **MAPE (Mean Absolute Percentage Error)**: This metric expresses accuracy as a percentage. The MAPE for our model is 0.89%, indicating that, on average, the model's predictions are off by 0.89% from the actual values. This low percentage signifies high accuracy in the model's predictions.

- **RMSPE (Root Mean Squared Percentage Error)**: This metric is similar to the MAPE but gives more weight to larger errors. The RMSPE for our model is 1.12%, which is also very low, indicating that the model performs well even when accounting for larger prediction errors.

As we can see below, the histograms of estimated and actual values ​​also covers itself in general.
![image](https://github.com/user-attachments/assets/3479404d-91ac-4995-bb8a-f8bb54589c7e)

These metrics demonstrate that **the model has a high level of accuracy and reliability in predicting** the electrical energy output of the Combined Cycle Power Plant.

## Contributing
Contributions are welcome! Please do not hesitate to contact me on LinkedIn!

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
