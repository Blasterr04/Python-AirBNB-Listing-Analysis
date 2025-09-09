# Airbnb Listings EDA Project  

---

## 📌 Project Overview
This project focuses on performing **Exploratory Data Analysis (EDA)** on Airbnb listings to identify key patterns and insights. The analysis covers listing prices, room types, host behavior, and availability trends. Libraries such as **Pandas, NumPy, Matplotlib, and Seaborn** are used for data cleaning, visualization, and statistical exploration.  

---

## 🎯 Objectives
- Examine **room types, pricing, and availability** across different areas.  
- Explore **host activities** and multi-listing behaviors.  
- Detect and handle **outliers in rental prices**.  
- Provide **data-driven recommendations** for both guests and hosts.  

---

## 📂 Dataset
The dataset contains **20,765 entries and 22 features**, including:  
- **id**: Unique identifier for each listing  
- **name**: Title of the Airbnb listing  
- **host_name**: Name of the host  
- **neighborhood_group**: Borough where the listing is located  
- **latitude / longitude**: Geographical coordinates  
- **price**: Nightly rental price  
- **room_type**: Type of accommodation (entire home, private room, etc.)  
- **reviews_per_month**: Average reviews per month  
- **availability_365**: Number of days available in a year  

---

## 🔄 Workflow

### 1. Data Cleaning
- Addressed missing values in `price`, `neighborhood`, and `beds`.  
- Converted `last_review` to **datetime** format.  
- Handled extreme price values by capping prices above $1,000.  

### 2. Exploratory Data Analysis
- **Room type distribution** → Bar plots showing popularity of different room types.  
- **Neighborhood insights** → Borough-wise price analysis, highlighting variations.  
- **Availability trends** → Heatmaps illustrating relationships among availability, price, and reviews.  
- **Price distribution** → Histograms to understand typical pricing ranges.  
- **Host activity** → Boxplots to analyze hosts with multiple listings.  
- **Review patterns** → Pair plots for review counts, price, and availability.  

### 3. Visualization
- **Pairplot** → Relationships among `price`, `availability`, and `reviews`.  
- **Heatmap** → Correlations between numerical variables.  
- **Histograms & Boxplots** → Identifying outliers in price.  
- **Bar Charts** → Distribution of room types and neighborhood groups.  

---

## 📊 Key Insights
1. **Pricing Trends**  
   - **Manhattan** listings are the most expensive, with Brooklyn following next.  
   - **Entire homes/apartments** generally cost more than private/shared rooms.  

2. **Room Types**  
   - **Entire homes/apartments** dominate the listings, while **private rooms** provide affordable alternatives.  

3. **Outliers**  
   - A small number of listings priced at **$10,000+** distort the overall distribution and should be filtered.  

4. **Availability**  
   - Listings with **high availability** tend to be cheaper and receive more reviews.  

5. **Host Behavior**  
   - Certain hosts manage **multiple properties**, reflecting professional hosting practices.  

---

## ⚙️ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   ```

2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Open and run the Jupyter Notebook:


## 💡 Recommendations

For Guests
- Choose listings with higher availability and consistent reviews for reliability.
- Consider private rooms outside Manhattan for more budget-friendly stays.

For Hosts
- Maintain good availability and actively engage with reviews to improve visibility.
- Price competitively within the neighborhood to attract more bookings.


## 🚀 Future Work
- Apply machine learning models to predict listing prices.
- Perform sentiment analysis on customer reviews for deeper insights.
- Build an interactive dashboard with Plotly or Tableau for dynamic analysis.
