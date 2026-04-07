# Prompt Engineering and LLM Evaluation

This project contains two comprehensive Jupyter notebooks demonstrating advanced techniques in prompt engineering and Large Language Model (LLM) evaluation.

## Project Overview

This repository showcases practical applications of modern AI technologies, focusing on:
- **Prompt Engineering**: Crafting effective prompts for classification tasks
- **LLM Comparison**: Evaluating different language models for various use cases
- **Multimodal AI**: Integrating text and image processing capabilities

## Notebooks

### 1. `prompt_engineering_netacad.ipynb` - Prompt Engineering for Classification
A comprehensive tutorial on using LLMs for sentiment analysis and aspect-based sentiment analysis.

#### Key Features:
- **Sentiment Analysis**: Binary classification of movie reviews
- **Aspect-Based Analysis**: Fine-grained sentiment analysis for product features
- **Model Comparison**: OpenAI GPT-4o vs. Groq models
- **Evaluation Metrics**: F1-score, accuracy, confusion matrices
- **Multimodal Capabilities**: Image description and generation with DALL-E
- **Data Pipeline**: Complete workflow from raw data to model evaluation

#### Learning Outcomes:
- Understand prompt engineering best practices
- Implement few-shot learning techniques
- Evaluate LLM performance on classification tasks
- Work with real-world datasets (IMDB reviews)
- Use multiple LLM providers (OpenAI, Groq)

### 2. `sma.ipynb` - LLM Testing and Multimodal Applications
Hands-on exploration of various LLMs with focus on practical implementation and multimodal features.

#### Key Features:
- **Model Comparison**: Testing OpenAI GPT-5.2, GPT-4o-mini, and Groq models
- **API Integration**: Secure key management and API calls
- **Multimodal AI**: Image description and analysis
- **Performance Evaluation**: Speed and quality comparisons
- **LangChain Framework**: Modern LLM application development

#### Learning Outcomes:
- Set up and configure multiple LLM providers
- Implement secure API key management
- Compare model performance across different tasks
- Work with multimodal (text + image) AI applications
- Use LangChain for streamlined LLM interactions

## Prerequisites

### System Requirements:
- Python 3.8+
- Jupyter Notebook or JupyterLab
- Internet connection for API calls

### Required Packages:
Install dependencies using pip:
```bash
pip install "req"

install them accordingly while going trought the fils and cells
```

### API Keys Required:
Create a `.env` file in the project root with:
```
OPENAI_API_KEY=your_openai_api_key_here
GROQ_API_KEY=your_groq_api_key_here
```

#### Getting API Keys:
1. **OpenAI**: Visit [platform.openai.com](https://platform.openai.com) and create an account
2. **Groq**: Visit [groq.com](https://groq.com) and sign up for API access

## Installation and Setup

1. **Clone or download** this repository
2. **Install Python dependencies**:
   ```bash
   pip install langchain-openai langchain-groq python-dotenv datasets pandas numpy scikit-learn tiktoken tqdm requests pillow
   ```
3. **Set up environment variables**:
   - Copy `.env.example` to `.env` (if provided) or create a new `.env` file
   - Add your API keys as shown above
4. **Launch Jupyter**:
   ```bash
   jupyter notebook
   ```
5. **Open the notebooks** and run cells sequentially

## Usage Guide

### Running the Notebooks:

1. **Start with `sma.ipynb`** for basic LLM setup and testing
2. **Move to `prompt_engineering_netacad.ipynb`** for advanced prompt engineering
3. **Execute cells in order** - some cells depend on previous outputs
4. **Monitor API usage** - LLM calls incur costs based on token usage

### Expected Outputs:
- Text responses from various LLMs
- Performance metrics and evaluation results
- Generated images (DALL-E)
- Structured JSON outputs for image descriptions

## Project Structure

```
practical_act1/
├── prompt_engineering_netacad.ipynb  # Main prompt engineering tutorial
├── sma.ipynb                         # LLM testing and multimodal demo
├── pyproject.toml                    # Python project configuration
├── .env                              # Environment variables (create this)
├── student.png                       # Sample image for multimodal testing
├── output.png                        # Generated image output
├── rag.PNG                          # Additional project assets
└── README.md                         # This file
```

## Key Concepts Covered

### Prompt Engineering:
- Zero-shot vs. few-shot learning
- System messages and user prompts
- Structured output formatting
- Token optimization

### Multimodal AI:
- Image encoding for API transmission
- Vision-language model capabilities
- Structured image analysis
- Text-to-image generation

## Troubleshooting

### Common Issues:

1. **API Key Errors**:
   - Ensure `.env` file exists and contains correct keys
   - Check key format (no extra spaces or quotes)
   - Verify account has sufficient credits

2. **Import Errors**:
   - Install all required packages
   - Check Python version compatibility
   - Restart Jupyter kernel after installations

3. **Rate Limiting**:
   - Space out API calls to avoid hitting limits
   - Monitor usage on provider dashboards
   - Consider upgrading API plans for higher limits

4. **Image Processing Issues**:
   - Ensure image files exist in correct paths
   - Check image formats (PNG/JPEG supported)
   - Verify base64 encoding works correctly

### Performance Tips:
- Use smaller datasets for initial testing
- Cache results when possible
- Monitor token usage to control costs
- Use temperature=0 for consistent results

## Educational Context

This project is part of the IA/Distributed Intelligence course practical activities. It demonstrates real-world applications of AI technologies in:
- Natural Language Processing
- Computer Vision
- API Integration
- Data Science Workflows

## Acknowledgments

- OpenAI for GPT model access
- Groq for accelerated inference
- Hugging Face for datasets
- LangChain for LLM framework
- IMDB for review dataset