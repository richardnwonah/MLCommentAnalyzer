
# Sentiment Analysis of Website Comments using ML.NET

This project demonstrates a sentiment analysis application that classifies website comments as positive or negative using ML.NET. The application leverages binary classification to analyze comments and predict their sentiment.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Prediction](#prediction)
- [Contributing](#contributing)
- [License](#license)

## Overview

This sentiment analysis application is built using ML.NET, a machine learning framework for .NET developers. It trains a model on a labeled dataset of comments and then uses this model to predict the sentiment of new comments as either positive or negative.

![Sentiment Analysis Demo](https://github.com/richardnwonah/MLCommentAnalyzer/images/demo.png)

## Dataset

The dataset used for training and testing is a labeled dataset containing comments with corresponding sentiment labels. The dataset is stored in the `Data` directory and is loaded during the training phase.

## Installation

To run this project, ensure you have the following installed:

- .NET SDK
- ML.NET

Clone the repository and navigate to the project directory:

```bash
git clone https://github.com/richardnwonah/MLCommentAnalyzer.git
cd your-repo
```

## Usage

To use the application, follow these steps:

1. **Load Data:** The data is loaded from the `yelp_labelled.txt` file.
2. **Train Model:** The model is trained using the loaded data.
3. **Evaluate Model:** The model is evaluated for accuracy and other metrics.
4. **Predict Sentiment:** Use the trained model to predict the sentiment of individual comments or a batch of comments.

## Model Training

The model is trained using the `SdcaLogisticRegression` algorithm provided by ML.NET. The text data is first featurized using the `FeaturizeText` transformer, and then the logistic regression algorithm is applied.

![Model Training](https://github.com/richardnwonah/MLCommentAnalyzer/images/training.png)

## Evaluation

The model is evaluated on a test dataset, and key metrics like Accuracy, AUC (Area Under Curve), and F1 Score are displayed to assess its performance.

![Model Evaluation](https://github.com/richardnwonah/MLCommentAnalyzer/images/evaluation.png)

## Prediction

The application provides methods to predict sentiment for single comments as well as a batch of comments. The predicted sentiment, along with the probability, is displayed for each comment.

![Prediction Results](https://github.com/richardnwonah/MLCommentAnalyzer/images/prediction.png)

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
