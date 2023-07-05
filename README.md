# Meteor Shower Prediction Jupyter Project

This Jupyter project aims to predict the best meteor shower viewing based on the given city. By utilizing historical meteor shower data and astronomical information, the project provides insights into the most favorable dates for observing meteor showers from specific cities.

## Table of Contents
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Methods](#methods)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
Meteor showers occur when the Earth passes through the debris trail left by a comet or asteroid. This project leverages historical data on meteor showers, city information, and astronomical data to predict the best meteor shower viewing based on a given city. The prediction is made using a function that selects the most suitable meteor showers and determines the optimal viewing dates.

## Installation
To use this project, follow these steps:

1. Clone the repository to your local machine.
2. Install the required dependencies by running the command `pip install -r requirements.txt`.
3. Launch Jupyter Notebook using the command `jupyter notebook`.
4. Open the project notebook `predicting meteorshowers.ipynb`.

Note: Ensure you have Python and Jupyter Notebook installed on your machine.

## Usage
The Jupyter Notebook provides a step-by-step guide on how to use the `predict_best_meteor_shower_viewing(city)` function to obtain the best meteor shower viewing predictions. It explains the function's parameters, input requirements, and provides example usage. You can run the notebook cells to see the function in action with different cities.

## Data
The project utilizes various datasets, including historical meteor shower observations, city information, moonphases and constellations. These datasets provide the necessary information for predicting the best meteor shower viewing. They are included in this repository and can be easily downloaded for further uses.

## Methods
The core method used in this project is the `predict_best_meteor_shower_viewing(city)` function. This function predicts the best meteor shower viewing based on the given city. Here's how it works:

1. Data preprocessing: The function checks if the given city is available in the dataset. If not, it returns an error message. The latitude of the city is extracted from the dataset.
2. Constellation selection: Constellations are selected based on the latitude range that includes the given city.
3. Meteor shower prediction: For each constellation in the selected list, the corresponding meteor shower, start date, and end date are retrieved from the dataset. Moon phases within the meteor shower date range are extracted.
4. Best viewing date: The date with the lowest moon phase percentage is determined as the best viewing date for each meteor shower.
5. Result generation: A string is constructed with the meteor shower name, constellation, and best viewing date for each meteor shower.
6. Return: The final string containing the meteor shower predictions is returned.

The Jupyter Notebook provides detailed code.

## Results
The results of this project are the predictions of the best meteor shower viewing based on the given city. By using the `predict_best_meteor_shower_viewing(city)` function, users can obtain information on the most suitable dates for observing meteor showers from specific cities. The predictions are based on historical data and astronomical information.

## Contributing
Contributions to this project are welcome. If you find any issues, have suggestions for improvements, or would like to contribute new features, please submit a pull request. Follow the existing coding style and provide clear commit messages.
