<<<<<<< HEAD
# Career Path Recommendation System

This project is a Career Path Recommendation System built with a React frontend and a Django backend. The system is implemented in four main steps:

1. **User Registration and Quiz**
2. **Machine Learning Prediction**
3. **Sentiment Analysis (NLP)**
4. **Chatbot Assistant**
5. **Voice Assistant**

## Features

1. **User Registration and Quiz**
   - After successful registration, the user is redirected to the quiz page.
   - The user answers 19 quizzes.
   - The user is automatically redirected to the prediction page to see their career job role based on their answers.

2. **Machine Learning Prediction**
   - The prediction is made using a machine learning model.
   - The model suggests a career path for the user based on their quiz answers.

3. **Sentiment Analysis**
   - If the user is not satisfied with the prediction, they can provide feedback.
   - An NLP model predicts whether the feedback is positive or negative using the NLTK library.
   - The sentiment (positive or negative) is displayed to the user.

4. **Chatbot and Voice Bot**
   - The chatbot responds to custom data queries.
   - Implemented using Google Gemini API, LangChain, and FAISS as the Vector-DB.
   - Google Gemini is used for word embeddings.
   - The voice bot is implemented with the React Speech Recognition library, FAISS DB, LangChain, and Gemini.

## Technologies Used

- **Frontend:**
  - React
  - React Speech Recognition

- **Backend:**
  - Django
  - DRF
  - NLTK
  - LangChain
  - FAISS
  - Google Gemini API

- **Database:**
  - FAISS (Vector-DB)
  - SQL

## Installation

### Prerequisites

- Node.js and npm
- Python 3.x and pip
- Django
- NLTK

### Backend Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/mani1854/career-path-recommendation-system.git
    cd career-path-recommendation-system/Prediction
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    venv\Scripts\activate
    ```

3. Install the dependencies:
    ```bash
    pip install -r requirements.txt
      ```
4. Create .env file inside the Prediction folder:

   GOOGLE_API_KEY = "YOUR_API_KEY"

5. Run the Django server:
    ```bash
    python manage.py migrate
    python manage.py runserver
    ```

### Frontend Setup

1. Navigate to the frontend directory:
    ```bash
    cd ../Frontend
    ```

2. Install the dependencies:
    ```bash
    npm install
    ```

3. Run the React development server:
    ```bash
    npm run dev
    ```

## Usage

1. Open your browser and navigate to `http://localhost:5173`.
2. Register as a new user.
3. Complete the quiz to receive a career path recommendation.
4. Provide feedback on the prediction to see the sentiment analysis.
5. Use the chatbot for custom queries.
6. Interact with the voice bot for voice commands.

## Deployment

### Backend (Django) - Options
- **Azure App Service** – The project includes a GitHub Actions workflow (`.github/workflows/main_ai-personal-assistant.yml`). To use it: (1) Create an Azure Web App named `career-path-recommendation` or update the `app-name` in the workflow, (2) Add `AZUREAPPSERVICE_PUBLISHPROFILE_*` to your GitHub repo Secrets, (3) Push to the `main` branch.
- **Railway / Render / Heroku** – Create a new web service, point it to your repo, set the start command to `python manage.py runserver` (or use gunicorn for production), and add `GOOGLE_API_KEY` and database env vars.

### Frontend (React/Vite) - Options
- **Vercel** – Connect your repo, set root directory to `Frontend`, build command `npm run build`, output directory `dist`. Add `VITE_API_URL` if your backend is elsewhere.
- **Netlify** – Same as above; root `Frontend`, build `npm run build`, publish `dist`.
- **GitHub Pages** – Run `npm run build` in `Frontend`, deploy the `dist` folder. You’ll need to set the correct base URL for the SPA.

### Full-Stack Tips
- Point the frontend `API_URL` (or equivalent) to your deployed backend URL.
- Add CORS allowed origins in Django `settings.py` for your frontend domain.
- Use environment variables for `GOOGLE_API_KEY`, `SECRET_KEY`, `DEBUG`, and database config in production.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes. 
=======
# career-path-recommendation-system
>>>>>>> 4a6db6fe99cb55ba06f1d5776b14152ea5ca19ac
