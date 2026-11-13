# User Segmentation & Clustering App

An interactive **Streamlit** web application powered by **PyCaret** and **Plotly** that assigns users to clusters based on demographic and lifestyle survey data, then visualizes the characteristics of their matched group.

## Key Features
- **Real-Time Cluster Prediction:** Uses a pre-trained `pycaret.clustering` pipeline (`welcome_survey_clustering_pipeline_v2`) to classify new user inputs on the fly.
- **Persona Matching:** Maps predicted cluster IDs to human-readable segment names and descriptions stored in JSON.
- **Interactive Data Visualizations:** Dynamically renders **Plotly Express** histograms comparing age, education level, favorite animals, preferred places, and gender distribution within the matched cluster.
- **Performance Optimization:** Implements `@st.cache_data` for model loading, dataset inference, and metadata parsing.

## Tech Stack
- **Python 3**
- **Streamlit** (UI & caching)
- **PyCaret** (Clustering model inference)
- **Pandas** (Data manipulation)
- **Plotly Express** (Interactive charts)