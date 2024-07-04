# lucksyatudu.github.io

### tziyur ###

## Description
    Generative AI based resource generator for churches to optimize, streamline and smoothen Social Media handeling experience.

    Uses Gemini to perform following tasks:
        - Daily Bible verse Generation: Generates bible verses by taking into account holidays and church events, making sure no verse gets repeated for a default of 365 days.
        - Caption Creation for Sermon: Summarizes sermon notes in 50-100 words, appropriate for Facebook and Instagram captions.

## Technology & Tools
    Python: Programming Language for all backend code
    FastAPI: Web API Framework
    Google Gemini: Generative AI for Text Generation Models
    Bible Gateway API: For comparing various transations
    API Ninjas API: For holiday lists for different countries

## Installation and Run
# create environment
    ```bash
        python3 -m venv env
        printf "\n # Adding this command to read local .env file" >> env/bin/activate
        printf "\nexport \$(grep -v '^#' .env | xargs)" >> env/bin/activate
    ```

# .env file contents
    PYTHONPATH
    GOOGLE_APPLICATION_CREDENTIALS
    GOOGLE_API_KEY
    HUGGING_FACE_TOKEN
    API_NINJAS_KEY
    UNSPLASH_APPLICATION_ID
    UNSPLASH_ACCESS_KEY
    UNSPLASH_SECRET_KEY

# installing dependencies
    ```bash
        pip install -r requirements.txt
    ```

# run server
    ```bash
        uvicorn main:app --reload
    ```
