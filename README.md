# Animal Ethics LLM Experiment

This project evaluates stated vs revealed preferences in LLMs using animal ethics.

## Setup

### Using uv (Recommended)

1. Install uv if you haven't already:
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

2. Create a virtual environment and install dependencies:
```bash
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
uv pip install -r requirements.txt
```

Or install dependencies directly:
```bash
uv pip install openai python-dotenv matplotlib
```

3. Set up your OpenRouter API key:
Create a `.env` file in the project root:
```bash
echo "OPENROUTER_API_KEY=your_actual_api_key_here" > .env
```

Or manually create `.env` with:
```
OPENROUTER_API_KEY=your_actual_api_key_here
```

4. Run the experiment:
```bash
python experiment.py
```

### Using pip (Alternative)

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Set up your OpenRouter API key (same as above)

3. Run the experiment:
```bash
python experiment.py
```

## Results

Results will be saved to:
- `results/proxy_rankings.json` - Raw responses and parsed rankings
- `results/proxy_rankings_comparison.png` - Visualization comparing rankings across models

