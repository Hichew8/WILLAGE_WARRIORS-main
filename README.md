# Introducing: Caduceo 🏥

## About the Project 📊

**Caduceo** is a comprehensive healthcare cost estimator and data analysis platform designed to bring transparency and efficiency to the healthcare industry. Built using Streamlit, Caduceo integrates seamlessly with MongoDB and Snowflake to provide real-time data on medical procedure costs, insurance rates, and hospital ratings. The platform offers a user-friendly interface with features such as a cost estimator, an intelligent chatbot powered by LLaMA for personalized assistance, and a MongoDB data viewer for in-depth analysis.

## Inspiration 💡

The inspiration for Caduceo came from the need for greater transparency in healthcare costs. Patients often face difficulties in understanding and comparing the costs of medical procedures, which can lead to unexpected expenses and financial stress. By providing a tool that offers clear and accurate cost information, we aim to empower patients, healthcare providers, and insurers to make informed decisions and improve the overall healthcare experience.

## How We Built Caduceo 🛠️

Caduceo was built using the following technologies and steps:

1. **Streamlit**: We used Streamlit to create the web application, providing a clean and interactive interface for users.
2. **MongoDB**: We connected to MongoDB using the `pymongo` library to fetch data from various collections, such as `apccosts`, `ccr`, `cptcosts`, `hospitalcost`, and `hospitalratings`.
3. **Snowflake**: We integrated Snowflake to fetch median rates and unique payers for healthcare procedures.
4. **LLaMA**: We implemented a chatbot powered by LLaMA to provide personalized assistance and enhance user interaction.
5. **OCR Parsing with Computer Vision**: We integrated OCR (Optical Character Recognition) technology to extract text from uploaded images, enhancing the data input process.
6. **Data Formatting**: We applied formatting functions to ensure that monetary values are displayed with commas, while other data types, such as codes, remain unaltered.

## Challenges We Faced 🚧

Building Caduceo was not without its challenges. Some of the key challenges we faced include:

- **Data Integration**: Integrating data from multiple sources (MongoDB and Snowflake) and ensuring consistency and accuracy.
- **Real-Time Data Fetching**: Implementing efficient data fetching mechanisms to provide real-time information without compromising performance.
- **Chatbot Integration**: Integrating the LLaMA chatbot and handling streaming responses to provide a seamless user experience.
- **OCR Parsing**: Implementing OCR technology to accurately extract text from images and integrate it into the platform.
- **Data Formatting**: Ensuring that monetary values are formatted correctly while maintaining the integrity of other data types, such as codes.

## Accomplishments that We're Proud Of 🏆

- Successfully integrating multiple data sources to provide comprehensive and accurate healthcare cost information.
- Developing a user-friendly interface that simplifies the process of estimating healthcare costs and analyzing data.
- Implementing a robust chatbot powered by LLaMA to assist users with personalized queries and enhance their experience.
- Integrating OCR technology to streamline the data input process and improve user interaction.

## What We Learned 📚

- The importance of data consistency and accuracy when integrating multiple data sources.
- Techniques for optimizing real-time data fetching to ensure a smooth user experience.
- Best practices for developing and integrating chatbots to provide meaningful and interactive user assistance.
- Effective methods for implementing OCR technology to enhance data extraction and input processes.

## Conclusion 🎯

Caduceo is a powerful tool designed to bring transparency and efficiency to the healthcare industry. By providing real-time data on medical procedure costs, insurance rates, and hospital ratings, Caduceo empowers patients, healthcare providers, and insurers to make informed decisions. We are excited to continue improving and expanding Caduceo to further enhance the healthcare experience for all users.

## What's Next for Caduceo 🚀

- Expanding the dataset to include more medical procedures and insurance providers.
- Enhancing the chatbot's capabilities to handle more complex queries and provide even more personalized assistance.
- Implementing additional features such as predictive analytics and trend analysis to offer deeper insights into healthcare costs and trends.

## Technical Documentation 📑

### Installation

To run Caduceo locally, follow these steps:

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/caduceo.git
    cd caduceo
    ```

2. **Create a virtual environment**:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

4. **Set up environment variables**:
    Create a `.env` file in the root directory and add the necessary environment variables for MongoDB, Snowflake, and any other services.

5. **Run the Streamlit application**:
    ```sh
    streamlit run backend/streamlit_app.py
    ```

### Key Modules

- **streamlit_app.py**: The main Streamlit application that sets up the web interface and handles user interactions.
- **ocr.py**: Contains functions for analyzing images and extracting text using OCR technology.
- **llama_integration.py**: Manages the integration with the LLaMA chatbot, including initializing the model and handling user inputs.
