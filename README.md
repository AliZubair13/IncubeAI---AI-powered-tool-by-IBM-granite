# IncubeAI---AI-powered-tool-by-IBM-granite
**Inqube AI**  

**Tagline**: Uncover limitless product insights from every angle...  

**Overview**:  
Inqube AI is a sophisticated competitor analysis tool tailored to assist businesses, startups, and entrepreneurs in gaining comprehensive insights into their competitors' products and services. Powered by AI and machine learning, the tool automates the collection, analysis, and visualization of data from diverse sources, including e-commerce platforms, websites, and YouTube. It offers actionable insights that empower users to make informed decisions, identify market opportunities, and enhance their strategies.

### **How Inqube AI Functions**  
Inqube AI, leveraging the IBM Granite Model, is designed to provide in-depth competitor insights. Here's a breakdown of its workflow:  

**Step 1: User Input**  
Users provide the following information:  

- **Product Name**: The name of the product or service for analysis  
- **Country Code**: A two-letter country code (e.g., US, IN) for region-specific results  
- **Search Parameters**:  
  - Number of search results to analyze  
  - Number of YouTube videos to analyze  
  - Number of YouTube comments per video to analyze  
  - Type: Choose ‘Product’ or ‘Service’ for precise analysis  

**Step 2: Web Search**  
The Serper tool performs a web search for product/service details, including:  

- Product name  
- Price  
- Product page link  
- Product description snippet  
- Seller information  
This generates a list of competitor products/services for further analysis.  

**Step 3: Web Scraping**  
The product links from Serper are processed using Crew AI’s ScrapeWebsiteTool. This tool:  

- Scrapes detailed data from product web pages  
- Extracts key information such as descriptions, features, pricing, and customer reviews  

**Step 4: YouTube Analysis**  
The product name is sent to the YouTube API to:  

- Find relevant videos for the product/service  
- Extract video transcripts using the youtube_transcript_api Python library  
- Gather comments from the videos for sentiment analysis  
This step helps in understanding customer sentiment and trends through video content and feedback.  

**Step 5: AI Analysis**  
The collected data, including video transcripts, scraped content, and product details, is processed by the IBM Granite Model (granite-3-8b-instruct). The model provides a detailed analysis with:  

- **SWOT Analysis**: Strengths, Weaknesses, Opportunities, and Threats  
- **Pros and Cons**: Key advantages and disadvantages of the product/service  
- **Sentiment Analysis**: Insights from YouTube comments (positive vs. negative)  
- **Price and Rating Analysis**: Competitive pricing and customer satisfaction metrics  
This analysis is repeated for each search result specified by the user.  

**Step 6: Final Output**  
The insights generated from all analyzed data are consolidated using the IBM Granite Model. The final output includes:  

- **Visualizations**:  
  - Bar graphs to compare pricing, ratings, and offers across competitors  
  - Pie charts to display sentiment distribution (positive vs. negative comments)  
- **Startup Recommendations**:  
  - Suggestions for launching a new product/service, including unique features, pricing strategies, marketing tips, potential risks, and solutions  

### **Key Features**  

- **Competitor Analysis**: Detailed analysis of competitor products/services  
- **YouTube Insights**: Extracts video transcripts and comments for sentiment analysis  
- **AI-Powered Insights**: Generates SWOT analysis, pros/cons, and actionable recommendations  
- **Interactive Visualizations**: Bar graphs and pie charts for comparison and understanding  
- **Customizable Inputs**: Adjust search parameters for tailored analysis  

### **Why Inqube AI?**  
Inqube AI integrates web scraping, YouTube analysis, and AI-driven insights to provide an all-encompassing competitor analysis tool. Whether launching a new product, refining your strategy, or exploring the market, Inqube AI offers valuable insights to help you stay ahead of the competition.

---

### **Setup**  
**Prerequisites**:  
- Python 3.8 or higher  
- Streamlit  
- Plotly  
- Requests  
- YouTube Transcript API
