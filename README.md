

````markdown
# Google AI Task Decomposition with Gemini 2.0 Flash

This Streamlit app uses Google's **Gemini 2.0 Flash** model to decompose high-level tasks into smaller, manageable subtasks.

## Setup

### 1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/google-ai-task-decomposition.git
   cd google-ai-task-decomposition
````

### 2. Create a virtual environment and activate it:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies:

```bash
pip install -r requirements.txt
```

### 4. Set up your Google Cloud credentials:

To find the details required for the `aiplatform.init()` function (like `project`, `location`, and `credentials`), you'll need to navigate to the Google Cloud Console and the Google Cloud AI Platform section. Below are the steps to get these details:

#### 1. Google Cloud Project ID

The **Project ID** is the unique identifier for your Google Cloud project. Here’s how to find it:

1. Go to **Google Cloud Console**: [Google Cloud Console](https://console.cloud.google.com/).
2. Navigate to the **Project Dashboard**: If you are not already in your project, click the project dropdown at the top of the page and select the project you are using.
3. **Find the Project ID**: Once you're in your project, you can find the **Project ID** listed under the **Project Info** section on the Dashboard or in the **IAM & Admin > Settings** page.

#### 2. Location (Region)

Google AI services like **Vertex AI** are available in multiple regions. For example, `us-central1` is one of the common regions used for deploying machine learning models in Google Cloud.

To find the available regions:

1. **Go to the Vertex AI Page**: In the Google Cloud Console, search for **Vertex AI** or navigate to the **AI & Machine Learning** section.
2. **Select a Region**: When creating an AI model or setting up an endpoint, you will choose a region for deployment. For example, `us-central1`, `europe-west4`, etc.

   * You can see the available regions for Vertex AI by visiting [Google Cloud Regions Documentation](https://cloud.google.com/about/locations).

For most use cases, `us-central1` works well as a default, but you can select other regions based on your needs and the geographic availability of the model.

#### 3. API Key

You can find your **API Key** in the **Google AI Studio** at the following URL:
[Google AI Studio API Keys](https://aistudio.google.com/app/api-keys).

* Copy the **API Key** from the AI Studio page.
* Set the environment variable for your API key:

  ```bash
  export GOOGLE_API_KEY="YOUR_GOOGLE_API_KEY"
  ```

### 5. Run the Streamlit app:

```bash
streamlit run app.py
```

### 6. Enter a task in the app, and the model will break it down into manageable subtasks.

## Requirements

* `streamlit`
* `crewai`
* `google-cloud-aiplatform`

## Here’s the repository structure:

google-ai-task-decomposition/
├── app.py           # Main Streamlit app code
├── README.md        # Documentation
├── requirements.txt # Project dependencies

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

````
