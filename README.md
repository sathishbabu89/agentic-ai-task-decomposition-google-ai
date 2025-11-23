````markdown
# Google AI Task Decomposition with Gemini 2.0 Flash

This Streamlit app uses Google's **Gemini 2.0 Flash** model to decompose high-level tasks into smaller, manageable subtasks. 

## Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/google-ai-task-decomposition.git
   cd google-ai-task-decomposition
````

2. Create a virtual environment and activate it:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Set up your Google Cloud credentials:

   * Obtain your **Google API Key** from the [Google AI Studio](https://aistudio.google.com/app/api-keys).
   * Set the environment variable for your API key:

     ```bash
     export GOOGLE_API_KEY="YOUR_GOOGLE_API_KEY"
     ```

5. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```

6. Enter a task in the app, and the model will break it down into manageable subtasks.

## Requirements

* `streamlit`
* `crewai`
* `google-cloud-aiplatform`

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

````

**c) `requirements.txt`**: Add the dependencies for the project.

```text
streamlit
crewAI
google-cloud-aiplatform
````

#### 4. **Commit and Push the Code**

Once you've added these files, you can commit and push your changes to GitHub.

```bash
git add .
git commit -m "Initial commit for Google AI Task Decomposition app"
git push origin main
```

### Conclusion

You now have a GitHub repository with your working Streamlit app code for **task decomposition using Google’s Gemini 2.0 Flash** model. The repository includes documentation on how to set up and use the app.

Here’s the repository structure:

```
google-ai-task-decomposition/
├── app.py           # Main Streamlit app code
├── README.md        # Documentation
├── requirements.txt # Project dependencies
```

Feel free to share the link to the repo with others, and let me know if you need any help with further steps or additions to the project!
