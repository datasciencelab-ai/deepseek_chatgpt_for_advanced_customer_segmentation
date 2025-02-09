# Using DeepSeek and chat GPT to Perform Advanced Customer Segmentation as a Data Scientist

### Youtube Video Link: https://www.youtube.com/watch?v=kc9QG2h-Hys

## I. Overview

### **1. Main Idea**

DeepSeek enables anyone—regardless of technical expertise—to perform data science tasks such as **advanced customer segmentation** with ease. In this blog, we will also compare DeepSeek with OpenAI's **ChatGPT O1-mini** to evaluate their effectiveness in automating customer segmentation.

### **2. Key Takeaways**

- Learn how to use **DeepSeek** for customer segmentation.
- Understand how **AI can automate many data science tasks, allowing non-experts to leverage AI tools for data analysis**.
- Gain insights into real-world applications of **AI-driven customer segmentation**.
- Compare **DeepSeek vs. ChatGPT O1-mini** to understand their strengths and weaknesses in customer segmentation.

## II. Structure

### **1. Why This Matters**

- **DeepSeek and ChatGPT O1-mini are powerful AI tools**, comparable in many aspects. While DeepSeek specializes in data-driven tasks, ChatGPT O1-mini is known for its strong natural language processing and general AI capabilities.
- **Customer segmentation** helps businesses understand their customers better and design effective marketing strategies.
- Traditional segmentation methods are **time-consuming** and require advanced expertise, but **DeepSeek and ChatGPT O1-mini simplify this process** for everyone.

### **2. What You’ll Learn**

- How DeepSeek helps with **advanced customer segmentation**.
- A step-by-step demonstration using **real-world data**.
- The benefits and **limitations of AI-powered data science**.
- A comparative analysis of **DeepSeek vs. ChatGPT O1-mini** for data science tasks.

## III. Customer Segmentation

### **1. What is Customer Segmentation?**

Customer segmentation is the process of grouping customers into **meaningful categories** based on their behavior, demographics, or purchasing patterns.

- Traditional methods use clustering techniques like **K-Means, Hierarchical Clustering, and DBSCAN**.
- With **DeepSeek and ChatGPT O1-mini**, these tasks are automated and require minimal coding skills.

### **2. Why is Customer Segmentation Important?**

- Helps businesses **target the right audience** with personalized marketing strategies.
- Improves **customer retention and engagement**.
- Supports better decision-making in industries like **e-commerce, finance, and retail**.

## IV. Steps to Get Started

### **Step 1: Get Access to DeepSeek and ChatGPT O1-mini**

- Visit [**DeepSeek website**](https://chat.deepseek.com/) and [**ChatGPT O1-mini website**](https://openai.com/chatgpt/).
- Sign up (or log in) to access AI-powered tools.

### **Step 2: Set Up Your Analysis Environment and Data**

- **Environment:** Use Google Colab for quick access and easy coding.
- **Dataset:** Download customer purchase history data from [this online retail dataset](https://raw.githubusercontent.com/databricks/Spark-The-Definitive-Guide/refs/heads/master/data/retail-data/all/online-retail-dataset.csv).

### **Step 3: Follow Standard Data Science Steps**

1. Understand the dataset (overview and aggregation).
2. Preprocess the data.
3. Perform feature engineering.
4. Build the AI model using DeepSeek and ChatGPT O1-mini.
5. Analyze the results and extract insights.
6. Compare results from DeepSeek and ChatGPT O1-mini.
7. Show the potential business impact of your findings (e.g., how much revenue your segmentation strategy could generate).

## V. AI Prompts for Customer Segmentation

### **1. Perform Customer Segmentation Using DeepSeek and ChatGPT O1-mini**

```markdown
# Prompt 1:
You are a senior data scientist working on customer segmentation. Analyze the below data and give me a direction to cluster our customer.

Dataset: {{
https://raw.githubusercontent.com/databricks/Spark-The-Definitive-Guide/refs/heads/master/data/retail-data/all/online-retail-dataset.csv
}}

# Prompt 2:
You did a good job. Now follow the suggested instruction to build clustering model using Kmeans method. After building a model, you need to analyze the results, extract insights and assess the business impact.

# Advanced prompt (Generated using chat GPT 4o)
You are a senior data scientist working on customer segmentation. 

Follow the below instructions to do step by step analysis for the provided dataset. Show your thought in detail during each step and provide the full code in the end.

1. Provide basic information of dataset and summarize the dataset by following:
   - Identify key metrics, including:
     - Data period
     - Number of records
     - Number of unique products
     - Number of unique customers
     - Total purchase volume
     - Average and total unit price
     - Bar plot for top 10 most saled items

2. Preprocess the data:
   - Handle missing values
   - Remove duplicates

3. Perform feature engineering:
   - Extract relevant features for segmentation
   - Normalize and scale data if needed

4. Build the AI model
   - Implement a clustering model for customer segmentation.
   - Limit the clusters below 5

5. Analyze the results and extract insights:
   - Evaluate the segmentation output.
   - Explain the characteristics of each cluster.

6. Assess the business impact:
   - Estimate the potential revenue impact using segmentation result.
   - Ensure the caculated values are meaningful.

Additional requirements:
   - Ensure the code is fully executable without error to run in Google Colab.
   - Use `display()` instead of `print()` for DataFrames.
   - Add `print("=== <what will be shown> ===")` statements to clarify outputs.
   - Separate printed or plotted results with clear delimiters.
   - Filter unnecessary system or library warnings for a cleaner output.
  
Dataset: {{
https://raw.githubusercontent.com/databricks/Spark-The-Definitive-Guide/refs/heads/master/data/retail-data/all/online-retail-dataset.csv
}}
```

### **2. Additional Enhancements**

```markdown
# Prompt 3:
You did a good job. Now, Based on the clustering results, do the following tasks.

1. Calculate below statistic for each cluster
- Average and Sum of Quantity, Unit Price, Total Price
- Count of invoices
- Count of unique products
- Mean Invoice Count Per Product
- Number products count per invoice
- Unit price mean per invoice
- Total price mean per invoice
- Total price sum per invoice
- Quantity Sum per invoice
- Unit price mean per stock
- Quantity sum per stock
- Tototal price mean per stock
- Total price sum per stock

2. Visualize ALL calculated metrics using a radar plot
- Draw 2 plot one show the real values without scaled, and another show the values after converted into compareable scale
- Ensure that 1 plot displaying all clusters with clear view of each cluster

3. Provide an insight from the result
- Provide an meaningful insight for this result and what strategies we should take to maximize the potential revenue

Additional requirements:
- Ensure the code is fully executable in Google Colab.
- Ensure to calculate total price = Quantity x 'UnitPrice' before calculatation.
- Ensure the visualization is clear, well-labeled, and comparable in scale across clusters.
- Provide insights from the results and propose clear business strategies based on the analyzed data.
```

## VI. Results

### DeepSeek R1:
- Advantages: Delivers in-depth analytical results, providing a better understanding of the data.
- Disadvantages: Slower response time, especially when detailed analyses are requested.

### ChatGPT o3-mini:
- Advantages: Offers faster reasoning and superior code generation support.
- Disadvantages: Its analysis is not as in-depth as that provided by DeepSeek R1.
- Optimization Tip for Using ChatGPT: Break down large problems into smaller parts to receive more detailed and accurate responses.

## **VI. Conclusion**
Even without writing extensive code, both DeepSeek and ChatGPT deliver impressive results for data analysis and building customer segmentation models using K-Means. Personally, I find that DeepSeek R1 provides more comprehensive analyses, while ChatGPT o3-mini excels in speed and coding assistance. Depending on the specific needs of your project, you can choose the tool that best fits your requirements or even combine both for optimal results.
