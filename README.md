# Spam Email Detection using Machine Learning 

By [<b>Hepsi Rani</b>](https://www.linkedin.com/in/hepsi-rani-4b78a3344/)

<!-- TABLE OF CONTENTS -->
<details>
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#data-description">Data Description</a></li>
    <li><a href="#data-pre-processing">Data Pre-processing</a></li>
    <li><a href="#model-training-and-evaluation">Model Training and Evaluation</a></li>
    <li><a href="#model-deployment">Model Deployment</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#acknowledgements">Acknowledgments</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

Spam detection is the process of identifying and filtering out unwanted or unsolicited messages, typically in the form of emails or text messages. These messages are often sent by spammers or malicious actors with the intent of promoting a product, service, or website, or to trick the recipient into providing personal information or downloading malware.

This repository contains a Python script that uses various machine learning models to classify spam messages from ham messages. The model is trained on a popular dataset of spam emails, and we use multiple machine learning models for classification.

### Built With

- NumPy
- Pandas
- Matplotlib
- Seaborn
- Sklearn

You can install all the above-mentioned libraries at once by executing the following command:

```sh
pip install -r requirements.txt
```

## Getting Started

To get a local copy up and running, follow these simple steps.

### Installation

1. Clone the repo

   ```sh
   git clone https://github.com/Hepsi216/Spam_email_detection.git
   ```

2. Install the required libraries

   ```sh
   pip install -r requirements.txt
   ```

3. Open and execute the ```.ipynb``` file. After complete execution, you will get a ```.pkl``` file for project deployment.

## Data Description

We have utilized the Email-Spam dataset, which is publicly available on Kaggle. The dataset comprises a collection of 5,572 emails, each having two features: `Category` and `Message`.

- `Message`: Contains the actual text of the email.  
- `Category`: Distinguishes between Spam and Ham emails.

## Data Pre-processing

### Steps Done:

- Dropped the columns: `Unnamed: 2`, `Unnamed: 3`, and `Unnamed: 4`.
- Converted the `Category` column to binary values (0 for spam, 1 for ham).
- Split the dataset into training and testing sets using `train_test_split`.
- Transformed emails into numerical features using `TfidfVectorizer`.

The text data was cleaned, tokenized, vectorized, and then converted into training and testing formats for modeling.

## Model Training and Evaluation

We used multiple machine learning models to classify messages as spam or ham. Each model was trained using the `fit()` method and tested using the `predict()` method.

### Evaluation Metrics:
- Accuracy
- Precision
- Recall
- F1-Score

### Models Used:
- Logistic Regression
- K Nearest Neighbors
- Decision Trees
- Random Forest
- Stacking Model

## Model Deployment

The file `Spam Classification Deployment.py` contains the deployment code using Streamlit. Streamlit is a powerful open-source Python library for building data science web applications.

To run the deployment script:

```sh
python Spam Classification Deployment.py
```

![Deployment Screenshot](https://github.com/Hepsi216/Spam_email_detection/blob/main/Data%20Source/deployment.png)

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this project better, please fork the repo and create a pull request. You can also open an issue with the tag "enhancement". Don’t forget to star the project!

Steps:
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the GNU General Public License v3.0. See `LICENSE.txt` for more information.

## Acknowledgments

This project was inspired by the Kaggle dataset on Spam Email Detection. We also acknowledge the open-source Python libraries used and their respective contributors.

## Contact

Hepsi Rani  
[LinkedIn](https://www.linkedin.com/in/hepsi-rani-4b78a3344/)  
[GitHub Repository](https://github.com/Hepsi216/Spam_email_detection.git)