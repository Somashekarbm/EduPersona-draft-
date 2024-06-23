# EduPersona

Welcome to the Awesome Personalized Recommendation System Project! This project aims to build a recommendation system for PDF learning materials based on user interactions and content similarity.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Models Implemented](#models-implemented)
- [Evaluation](#evaluation)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

## Introduction

This project leverages collaborative filtering and content-based filtering techniques to recommend PDF learning materials to users based on their past interactions and content similarities. It integrates SQLite for storing metadata and user interactions, and uses libraries such as Surprise and scikit-learn for model building and evaluation.

## Features

- **Collaborative Filtering:** Utilizes user-item interactions to recommend items based on similar users' preferences.
- **Content-Based Filtering:** Recommends items similar to those a user has liked in the past, based on PDF metadata.
- **SQLite Database:** Stores PDF metadata and user interactions for seamless integration and data management.
- **Model Evaluation:** Cross-validates models to ensure robust performance using metrics like RMSE and MAE.
- **Dynamic Recommendations:** Recommends PDFs dynamically based on user inputs and interactions.

## Getting Started

### Prerequisites

Ensure you have Python 3.7+ installed along with the following libraries:

- pandas
- numpy
- scikit-learn
- surprise
- sqlite3

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Somashekarbm/EduPersona.git
   ```

## Usage

1. **Load Data:** Ensure your PDF metadata and user interactions are stored in SQLite database `pdfs.db`.
2. **Preprocess Data:** Clean and preprocess data as described in the project documentation.
3. **Model Building:**
   - Use collaborative filtering with Surprise library .
   - Implement content-based filtering using TF-IDF .
4. **Evaluate Models:** Cross-validate models to assess performance .
5. **Get Recommendations:** Use functions like `get_recommendations(pdf_title)` to get recommendations dynamically.

## Data

The project uses PDF metadata (title, keywords, difficulty, etc.) and user interactions (view, timestamp, rating) stored in the SQLite database `pdfs.db`.

## Models Implemented

1. **Collaborative Filtering:**
   - Uses Surprise library's SVD algorithm to predict ratings based on user-item interactions.

2. **Content-Based Filtering:**
   - Utilizes TF-IDF vectorization of PDF keywords to recommend similar items based on content.

## Evaluation

The models are evaluated using cross-validation techniques with metrics such as RMSE (Root Mean Squared Error) and MAE (Mean Absolute Error).

## Contributing

Contributions are welcome! Feel free to open issues or pull requests for bug fixes, enhancements, or new features.


## Acknowledgments

- Special thanks to the open-source communities behind pandas, scikit-learn, Surprise, and SQLite for their invaluable contributions.

---

Feel free to customize this README template further based on additional details specific to your project. It should serve as a comprehensive guide for users and contributors, outlining the project’s purpose, setup instructions, usage guidelines, and more.
