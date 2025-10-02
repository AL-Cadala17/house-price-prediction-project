# House Price Prediction Project

This is a full-stack web application that predicts house prices based on various features like size, number of bedrooms, and location. The backend is built with Python and Scikit-learn, served via a Flask API, and the frontend is a user-friendly interface built with Next.js.

## ✨ Features

-   **Accurate Predictions:** Utilizes multiple machine learning models (Linear Regression, Random Forest) to predict prices.
-   **Interactive UI:** A clean and simple web interface to input house features and get a price prediction.
-   **REST API:** A backend API that exposes the machine learning model for predictions.

## 🛠️ Tech Stack

### Backend
-   Python
-   Flask

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You need to have the following software installed on your machine:
-   [Python 3.8+](https://www.python.org/downloads/)
-   [Node.js v18+](https://nodejs.org/en/)

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/AL-Cadala17/house-price-prediction-project.git](https://github.com/AL-Cadala17/house-price-prediction-project.git)
    cd house-price-prediction-project
    ```

2.  **Set up the Backend:**
    Install the required Python packages from the root directory.
    ```sh
    pip install -r requirements.txt
    ```

3.  **Set up the Frontend:**
    Navigate to the `client` directory. Then, use your preferred package manager to install the dependencies.

    **Using npm (default):**
    ```sh
    cd client
    npm install
    ```
    **Or using Bun:**
    ```sh

    cd client
    bun install
    ```
    **Or using Yarn:**
    ```sh
    cd client
    yarn install
    ```

## 🏃‍♀️ Usage

To run the application, you need to start both the backend server and the frontend application in two separate terminals.

1.  **Run the Backend Server:**
    From the **root** directory (`house-price-prediction-project`), run:
    ```sh
    python app.py
    ```
    The API server will start on `http://127.0.0.1:8000/`.  

2.  **Run the Frontend Application:**
    Open a **new terminal** and navigate to the `client` directory. Then, use your preferred package manager to start the development server.

    **Using npm (default):**
    ```sh
    cd client
    npm run dev
    ```
    **Or using Bun:**
    ```sh
    cd client
    bun run dev
    ```
    **Or using Yarn:**
    ```sh
    cd client
    yarn dev
    ```
    The application will be available at `http://localhost:3000`. Open this URL in your web browser to use the app.

## 📂 Project Structure
```
house-price-prediction-project/
│
├── client/
│   ├── public/         # Static assets for the frontend
│   ├── src/            # Next.js source code (pages, components)
│   ├── next.config.ts  # Next.js configuration
│   └── package.json    # Frontend dependencies and scripts
│
├── dataset/
│   ├── house_dataset.csv       # Raw, original data
│   └── house_dataset_clean.csv # Cleaned data ready for training
│
├── models/
│   ├── house_scaler.pkl          # Saved scaler for feature transformation
|   ├── house_train_columns.json  # Saved list of training column names
│   ├── lr_model.joblib           # Saved Linear Regression model
│   └── rf_model.joblib           # Saved Random Forest model
│
├── .gitignore          # Specifies files for Git to ignore
├── app.py              # Main backend file: Flask server and API endpoints
├── model.py            # Script to define and train the machine learning models
├── process.py          # Script for data cleaning, preprocessing,feature engineering and scaling
├── requirements.txt    # List of Python dependencies for the backend
├── utils.py            # Helper functions used by other scripts
└── README.md           # Project documentation
```