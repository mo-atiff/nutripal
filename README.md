# NutriPal

[Link to my app](https://nutripal.streamlit.app/)

## Introduction
NutriPal is an AI-powered nutrition coach that helps users manage their dietary habits by generating customized recipes, predicting future meals, and providing nutritional information. It leverages the power of AI models such as those from OpenAI and Hugging Face to offer personalized recommendations based on user input and history.

## Table of Contents
- [Introduction](#introduction)
- [Table of Contents](#table-of-contents)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Dependencies](#dependencies)
- [Configuration](#configuration)
- [Documentation](#documentation)
- [Examples](#examples)
- [Hosted Application](#hosted-application)
- [Troubleshooting](#troubleshooting)
- [Contributors](#contributors)
- [License](#license)

## Installation
To install and run NutriPal locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/mo-atiff/story-generator.git
    cd story-generator
    ```

2. Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Create a `.env` file in the root directory with the following content:
    ```plaintext
    mongokey=your_mongodb_key
    huggingfaceapikey=your_huggingface_api_key
    ```

5. Run the application:
    ```bash
    streamlit run food.py
    ```

## Usage
1. Open the application in your web browser as directed by Streamlit.
2. Use the sidebar to log in or sign up.
3. Enter your Hugging Face API token in the provided field.
4. Upload an image of food or proceed without an image.
5. Enter health conditions and available kitchen ingredients.
6. Click "Generate Dish" to get a customized recipe.
7. Navigate to the "Predict next Food" or "Get Nutritional Info" pages using the sidebar.

## Features
- **User Authentication**: Log in or sign up to access personalized recommendations.
- **Image Upload**: Upload food images to detect ingredients.
- **Health Considerations**: Input health conditions to tailor recipes.
- **Environmental Impact**: Option to consider water footprint in recipes.
- **Recipe Generation**: Create detailed recipes based on available ingredients.
- **Meal Prediction**: Predict the next meal based on food consumption history.
- **Nutritional Information**: Get detailed nutritional information for recipes.

## Dependencies
- Streamlit
- Langchain
- HuggingFace Hub
- Spacy
- PIL
- Moviepy
- Pyttsx3
- Mutagen
- pymongo
- python-dotenv
- transformers

## Configuration
- **MongoDB Connection**: Required for user data storage and retrieval.
- **Hugging Face API Key**: Required for AI-powered functionalities.

## Documentation
For detailed documentation on using NutriPal, refer to the code comments and functions within `food.py`, `next_food.py`, and `nutrition.py`.

## Examples
### Generating a Customized Recipe
1. **Input**: "I have ripe tomatoes, fresh basil, garlic cloves, olive oil, chicken breast"
2. **Generated Recipe**: A detailed recipe using the provided ingredients.

### Predicting the Next Meal
1. **Input**: Food consumption history like "Breakfast: Eggs, Lunch: Salad, Dinner: Chicken"
2. **Predicted Meal**: AI-generated suggestion for the next meal based on past consumption patterns.

### Getting Nutritional Information
1. **Input**: Ingredients and instructions for a recipe.
2. **Nutritional Info**: Detailed nutritional content including proteins, carbohydrates, fats, vitamins, and minerals.

## Hosted Application
You can also try out NutriPal without any setup by visiting the hosted application:

[NutriPal on Streamlit](https://nutripal.streamlit.app/)

## Troubleshooting
If you encounter any issues, consider the following steps:
- Ensure that you have entered valid API keys for MongoDB and Hugging Face.
- Check the console for error messages and stack traces.
- Reload the application and try again.

## Contributors
- **Atif Shaik** - [GitHub Profile](https://github.com/mo-atiff)

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
