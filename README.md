# AI_real_estate_property_agents
An intelligent property recommendation system that leverages AI to streamline real estate search and analysis across multiple platforms.

## Overview

The AI Real Estate Agent is a sophisticated application that combines web data extraction via Firecrawl with intelligent analysis through OpenAI's language models. It helps users find properties matching their specific criteria while providing valuable market insights and investment recommendations. The application automates what would typically require hours of manual search across different real estate websites, delivering organized results and expert analysis in minutes.

## Features

- **Multi-Source Property Search**: Extracts relevant property listings from leading real estate websites including SquareYards, 99acres, and Housing.com
- **Customizable Search Criteria**: Filter by city, property type, category, and budget
- **AI-Powered Analysis**: Leverages OpenAI's models for detailed property evaluation and comparisons
- **Location Trend Analysis**: Provides price trends, rental yields, and investment potential for different localities
- **Intelligent Recommendations**: Suggests top properties with detailed reasoning and negotiation tips
- **User-Friendly Interface**: Clean Streamlit UI for intuitive interaction

## Installation

### Requirements

Create a `requirements.txt` file with the following dependencies:

```
agno
firecrawl-py==1.9.0
pydantic
streamlit
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

### Configuration

Before using the application, you'll need:

- **Firecrawl API Key**: Register at [Firecrawl](https://firecrawl.dev/) to obtain your API key
- **OpenAI API Key**: Sign up at [OpenAI Platform](https://platform.openai.com/) and create an API key

## Usage

1. Start the application:
   ```bash
   streamlit run app.py
   ```

2. In the sidebar:
   - Select the OpenAI model (o3-mini or gpt-4o)
   - Enter your API keys for Firecrawl and OpenAI

3. Configure your property search:
   - Enter the city name
   - Select property category (Residential/Commercial)
   - Choose property type (Flat/Individual House)
   - Set your maximum budget in Crores

4. Click "Start Search" to initiate the property search and analysis

5. Review the results:
   - Detailed property recommendations with analysis
   - Location trends with investment insights

## Example Output

### Property Recommendations

The application provides structured property analysis including:
- Selected properties matching your criteria
- Best value analysis comparing price per sq ft and amenities
- Location insights specific to property areas
- Top 3 recommended properties with detailed reasoning
- Property-specific negotiation strategies

### Location Trends

For each city, you'll receive:
- Summary of price trends for major localities
- Top performing areas based on price appreciation and rental yields
- Investment insights for different neighborhoods
- Specific recommendations for long-term vs. rental investments

## Technical Details

The application is built using:
- **Streamlit**: For the user interface
- **Firecrawl**: For extracting property data from multiple websites
- **Agno Agent & OpenAI**: For intelligent property analysis and recommendations
- **Pydantic**: For data validation and schema definition


## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Firecrawl](https://firecrawl.dev/) for providing the web data extraction capabilities
- [OpenAI](https://openai.com/) for the AI models used in property analysis
- [Streamlit](https://streamlit.io/) for the web application framework
