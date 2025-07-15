

📚 Book Recommender System
Project Overview
This project implements a personalized book recommendation system utilizing machine learning clustering techniques. The system aims to help users discover new books based on their reading preferences, by grouping similar books together and suggesting items from clusters aligned with the user's past interactions or expressed interests. The web application is built using Streamlit, providing an interactive and intuitive user interface.

Features
User-friendly Interface: An intuitive web interface built with Streamlit for searching and receiving recommendations.

Clustering-based Recommendations: Leverages a pre-trained machine learning model (model.pkl) to cluster books.

Personalized Suggestions: Provides recommendations based on existing book data and ratings.

Efficient Data Loading: Utilizes pickle to quickly load pre-processed data and the trained model.

Interactive Controls: Employs Streamlit's widgets for user input (e.g., selecting a book for suggestion).

Technologies Used
Programming Language: Python

Web Framework:

Streamlit (for building the interactive web application)

Machine Learning & Data Handling Libraries:

pickle (for serializing/deserializing Python objects like models and dataframes)

numpy (for numerical operations)

pandas (implicitly, as the .pkl files likely contain pandas DataFrames)

scikit-learn (implicitly, as model.pkl is likely a scikit-learn model)

Installation and Setup
To get this project up and running on your local machine, follow these steps:

Clone the Repository:

Bash

# Clone the repository
git clone https://github.com/satheeshyadav/book_recommender_system.git

# Go into the project directory
cd book_recommender_system


Run the Setup Script (Recommended):
The setup.sh script might automate environment creation and dependency installation.

Bash

bash setup.sh
If setup.sh doesn't exist or isn't functional, proceed with manual steps:

Manual Setup (if setup.sh is not used or fails):

Create a Virtual Environment:

Bash

python -m venv venv
# On Windows:
.\venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
(Note: Your screenshot shows env39, but venv is a common convention and often created by setup.sh.)

Install Dependencies:

Bash

pip install -r requirements.txt
(Ensure streamlit, numpy, and pandas (if used directly) are in your requirements.txt.)

Ensure Data and Artifacts are in Place:

Make sure your raw data files (BX-Book-Ratings.csv, BX-Books.csv, BX-Users.csv) are accessible, likely in the root directory as per your screenshot.

Verify that your pre-trained model and processed data (book_names.pkl, final_rating.pkl, model.pkl, book_pivot.pkl) are located in the artifacts/ directory. These files are crucial for the app.py to function, as it directly loads them. If these files are not present, you'll need to run your data preprocessing and model training scripts first (assuming you have them, e.g., scripts/preprocess_data.py, models/train_model.py).

Run the Streamlit Application:

From the root directory of the project (book_recommender_system), execute the Streamlit application:

Bash

streamlit run app.py
Access the Application:

Streamlit will automatically open a new tab in your default web browser, typically at http://localhost:8501 (as shown in your VS Code terminal).

Usage
Once the Streamlit application is running, you can:

Select a Book: Use the provided input interface to choose a book from the list.

Get Suggestions: The system will use the loaded model and data to provide book suggestions based on your selection.

Explore: Discover new titles based on the system's recommendations.

Website Screenshots
Here are some screenshots showcasing the user interface of the book recommender system:

Main Application Interface
A brief description of what this screenshot shows (e.g., "The primary interface of the book recommender system, showing the input selection and initial recommendations.").

<img width="960" height="600" alt="66666666" src="https://github.com/user-attachments/assets/5a1c7f4e-b266-4903-90a1-759c3493154b" />


Future Enhancements (Optional)
Integrate with external APIs (e.g., Google Books API, Goodreads API) for richer book data (cover images, detailed descriptions).

Implement user profiles and reading history tracking.

Explore different recommendation algorithms (e.g., collaborative filtering) to create a hybrid system.
Improve the user experience with more advanced Streamlit components or custom CSS.

Deploy the application to a cloud platform (e.g., Streamlit Community Cloud, Hugging Face Spaces).

Contributing (Optional)
We welcome contributions to improve this project! If you have suggestions, bug reports, or feature requests, please open an issue or submit a pull request.

License (Optional)
This project is licensed under the MIT License - see the LICENSE file for details.

Crucial Steps for You:

Replace YourUsername: Update https://github.com/YourUsername/book_recommender_system.git with your actual GitHub username.

Add Your Screenshots: Create an assets/ folder in your repository's root, place your actual screenshots there (e.g., main_app.png, recommendations.png), and update the image paths in the README.md accordingly.

Verify setup.sh: If your setup.sh doesn't fully automate setup, make sure to add specific instructions for what it does, or guide users through the manual venv and pip install steps.

Confirm requirements.txt: Double-check that your requirements.txt file lists all necessary libraries (streamlit, numpy, pandas, scikit-learn if used directly).

Ensure artifacts/ Content: The most important part is that artifacts/book_names.pkl, artifacts/final_rating.pkl, artifacts/model.pkl, and artifacts/book_pivot.pkl are correctly generated and present in your repository, as your app.py directly loads them.







