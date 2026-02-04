# MacroMicro Chart Analyst

A Streamlit chatbot that analyzes MacroMicro financial charts using Google's Gemini API with Google Search grounding.

## Features

- Load and display MacroMicro charts by URL
- Extract chart data including series names and latest values
- Chat interface for analyzing charts with Gemini AI
- Google Search grounding for real-time market information

## Setup

1. Install dependencies:
```bash
uv sync
```

2. Create `.streamlit/secrets.toml` with your Gemini API key:
```toml
GEMINI_API_KEY = "your-api-key-here"
```

3. Run the app:
```bash
uv run streamlit run main.py
```

## Usage

1. Enter a MacroMicro chart URL in the sidebar
2. Click "Load Chart" to fetch the chart data and preview
3. Ask questions about the chart in the chat interface

### Supported URL Formats

- `https://www.macromicro.me/charts/{chart_id}/{slug}`
- `https://www.macromicro.me/collections/{collection_id}/{collection_slug}/{chart_id}/{slug}`

### Examples

- `https://www.macromicro.me/charts/444/us-mm-gspc`
- `https://www.macromicro.me/collections/34/us-stock-relative/444/us-mm-gspc`
