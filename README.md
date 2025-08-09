🎓 Customer Admission Agent – IBM watsonx.ai Chatbot
This project is an AI-powered college admission assistant built using IBM watsonx.ai and Watson Machine Learning.
It responds to user conversations & queries and provides college admission-related information, such as the IIT admission process.

📌 Features
Responds to greetings like hi and hello.
Uses IBM watsonx.ai for natural language processing.
Searches for and answers admission-related queries.
Can be customized for any institution or domain.

🛠️ Requirements
Before running the notebook, ensure you have:
Python 3.9+
IBM Cloud account (Sign up here)
Provisioned watsonx.ai service
Cloud Object Storage for data (if needed for context retrieval - this project has RAGQuery tool being used)

The following Python libraries:
bash
Copy
Edit
pip install ibm_watsonx_ai
pip install ibm_boto3

🔑 IBM Cloud Credentials
You'll need the following credentials from IBM Cloud:
Variable Name	Description
API_KEY	IBM Cloud API key (keep this secret)
PROJECT_ID	Your watsonx.ai project ID
SPACE_ID	Deployment space ID (not secret, but don’t share with credentials)
VECTOR_INDEX_ID	Optional – for vector search integration
SOURCE_PROJECT_ID	Optional – for linking other projects

⚠️ Security Note:
Do not commit your API_KEY or other sensitive credentials to GitHub. Use .env files or GitHub Secrets.

🚀 Running the Project
Clone the repository:
bash
Copy
Edit
git clone https://github.com/yourusername/admission-agent.git
cd admission-agent

Create a .env file:
env
Copy
Edit
API_KEY=your_ibm_api_key
PROJECT_ID=your_project_id
SPACE_ID=your_space_id
Open the notebook:

bash
Copy
Edit
jupyter notebook "Customer Admission Agent.ipynb"
Run the cells in order.

📂 Project Structure
bash
Copy
Edit
.
├── Customer Admission Agent.ipynb  # Main notebook
├── README.md                       # Project documentation
└── requirements.txt                # Python dependencies

🧠 Customization
Modify greeting responses for your institution.
Update search prompts for a different college or domain.
Integrate a vector index for richer context-aware answers.

📜 License
MIT License – feel free to use and modify, but give credit.
