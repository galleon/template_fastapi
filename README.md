# FastAPI Video Frame Converter Service

This FastAPI service receives a video file, extracts the first frame, converts it to black and white, and sends the image back to the calling client, such as the Streamlit Video Frame Converter App.

## Installation

To set up and run this service, ensure you have Python 3.8 or higher installed on your system.

1. Clone this repository or download the source code.
2. Navigate to the directory containing the `fastapi_service.py` file.
3. Install Poetry for dependency management:
   
   ```bash
   pyenv virtualenv 3.10 template_fastapi
   pyenv local template_fastapi
   pip install poetry
   ```

4. Install the required dependencies using Poetry:

   ```bash
   poetry install
   ```

5. Activate the Poetry virtual environment:

   ```bash
   poetry shell
   ```

6. Start the FastAPI service:

   ```bash
   uvicorn fastapi_service:app --reload
   ```

   The service will be available at http://localhost:8000. It can now receive video files for processing from the Streamlit app.

   Ensure this service is running before attempting to upload a video in the Streamlit interface.

   For further assistance or to report issues, please open an issue in the project repository.
