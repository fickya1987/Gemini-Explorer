# Gemini-Explorer

This project is a chat interface developed using Streamlit to integrate with Google's cutting-edge large language model, Gemini, providing an accessible platform to explore and demonstrate the capabilities of advanced language model applications. 
This project serves as a practical introduction to the fusion of large language models and user-friendly interfaces.

## Requirements

- Python version 3.11x or above
- Streamlit [Streamlit Documentation](https://docs.streamlit.io/)
- Gcloud account
- Vertexai [Vertexai Documentation](https://cloud.google.com/vertex-ai)

## Task 1: 🌐 Enabling Google Cloud

- Go to the [Google Cloud Platform](https://cloud.google.com/free/?utm_source=google&utm_medium=cpc&utm_campaign=japac-IN-all-en-dr-BKWS-all-core-trial-EXA-dr-1605216&utm_content=text-ad-none-none-DEV_c-CRE_644159077391-ADGP_Hybrid+%7C+BKWS+-+EXA+%7C+Txt+~+GCP_General_core+brand_main-KWID_43700074766895886-aud-970366092687:kwd-6458750523&userloc_9062223-network_g&utm_term=KW_google%20cloud&gad_source=1&gclid=CjwKCAjw48-vBhBbEiwAzqrZVFHOq76jh9J0dgd2lwSHL3oF20yQX_sP4TvFoe6Nw7ofMguovMUk3BoChZ4QAvD_BwE&gclsrc=aw.ds) and Select "Get Started for free".
- Sign in using your Google Account and then provide the necessary details and complete the billing requirments.
- Accept the terms and conditions.
- Complete the payment process to initialize your Google Cloud Account.
- Create a new project (for instance "RadicalX - Gemini Explorer").
- Access the Google Cloud Console.
- Navigation -> Artificial Intelligence -> Vertex AI -> Enable All Recommended APIs

## Task 2: 🧬 Google Cloud Initialization

- Install the Google SDK using this [Link](https://cloud.google.com/sdk/docs/install).
- Run the following command to initialize the SDK:
  ```
  gcloud init
- Sign in using your Google Account credentials.
- Select an existing project or Create a new project (like "gemini-explorer")
- Set default compute region and zone (Optional Step)
- In your Google Cloud account, go to service accounts and create a service account for the project. Then, click on the account and create a new key in JSON format. Download this key and place it in your project folder.
- Then, go to IAM and create add "AI Platform Admin" as a role for the project.
- In the Command Line of your editor, type the following command to ensure google cloud authentication,
  ```
  set GOOGLE_APPLICATION_CREDENTIALS=your-key.json

## Task 3: ☁️ Setting up Google Gemini

- Install requirements.txt using the command
  ```
  pip install -r requirements.txt
- The requirements.txt installs the following frameworks/libraries
    * streamlit
    * google-cloud-aiplatform
    * vertexai
- This project utlizes Google's Gemini Pro LLM.
- Set the project_id in the code.

## Task 4: 📊 Streamlit Integration

- Integrate the LLM responses into the streamlit UI.
- Run the application using the command
  ```
  streamlit run filename.py

## Task 5: 🗣️ Adding Initial System Messages

- Personalize the LLM responses to create a seamless and interactive user interface.

![Gemini Explorer Chat Interface with multiturn conversation](https://github.com/user-attachments/assets/3d08eca7-7101-48fd-9b39-508f3f081fbf)


## Issues Faced

- ⚠️ **Issue 403: Permission Denied Error**: Check if you have provided project_id rather than project name in your code or if the service account is activated.
- Utilized "project_id" instead of project name to mitigate error.

## Acknowledgements

Special thanks to Mikhail Ocampo for the continued guidance on this AI Project during the internship.
