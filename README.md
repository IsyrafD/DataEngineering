# **ETL Process for Shopping Website Data (Group Project TTTC3213)**

This project demonstrates the **ETL (Extract, Transform, Load)** process using data scraped from the **Al-Ikhsan website**, focusing on product details such as ratings, discounts, and pricing. It is completed as part of the **TTTC3213 Group Assignment** for the academic term, adhering to the guidelines provided.

---

## **Project Overview**

### **Objective**
To extract, transform, and load product data from a shopping/business website and visualize insights for analysis.

### **Group Members**
1. **NUR AFRINA NABIHAH BINTI MOHD AZMI (A195030)**: Brand, Product Name  
2. **NURUL SYAFIKAH NATASYA BINTI MOHD SALLEH (A193668)**: Price, Discount  
3. **SITI NURSOLEHAH BINTI ZAMRI (A195524)**: Ratings, Reviews  
4. **ISYRAF DANISY BIN MAT ZAMRI (A193888)**: SKU, Description  
5. **MUHAMMAD NAJMI BIN NOR BAHRIN ()**: Installment, Product Image URL  

### **Dataset**
- **Website**: [Al-Ikhsan - Men’s Lifestyle Collection](https://al-ikhsan.com/collections/mens-lifestyle)
- **Records**: 100+ products scraped.

---

## **ETL Breakdown**

### **1. Extract (10 Points)**

1. **Dataset Selection**:
   - Chose the Al-Ikhsan website for its rich product data (e.g., ratings, discounts, prices).
   - Verified that scraping this site is legal and ethical.  

2. **Data Scraping**:
   - Scraped data using Python libraries: `BeautifulSoup`, `requests`.
   - Extracted attributes:  
     - Product details: Brand, Name, Price, Discount, SKU, Image URL.
     - Additional attributes: Ratings, Reviews, Description, Installment options.

3. **Record Count**:
   - Successfully collected **100+ product records** with all required attributes.

---

### **2. Transform (10 Points)**

1. **Data Cleaning**:
   - **Standardization**: Converted text (e.g., capitalization for brands/product names).
   - **Numerical Conversion**: Cleaned prices (removed non-numeric characters) and discounts (removed `%`).
   - **Rating Transformation**: Reformatted ratings into a clear scale (e.g., "4.5/5").
   - **Review Cleaning**: Summarized feedback by removing non-ASCII characters and counting emojis (e.g., thumbs-up count).

2. **Data Visualization**:
   - **Before Cleaning**:
     - Visualized unstructured ratings and inconsistent discount data in bar charts.
   - **After Cleaning**:
     - Cleaned and structured ratings (e.g., "4.5/5") and discounts (logical order) for clearer comparison.

---

### **3. Load (2 Points)**

- The cleaned data is saved into a **CSV file (`alikhsancleaned.csv`)**, which can be easily read by `pandas` or other tools.

---

### **4. Report (8 Points)**

1. **Experience Documentation**:
   - A detailed project write-up is published on [Medium](https://medium.com).
   - The Medium article includes:
     - **Code explanations**.
     - **Visualizations (before and after cleaning)**.
     - **GitHub repository link** to the project.

2. **Submission**:
   - Shared the **Medium link** and cleaned `.csv` file on **UKMFolio**.

---

## **Repository Structure**

```
├── Group_assignment_30__SEIS6.ipynb  # Main ETL process and code implementation
├── alikhsan.csv                      # Raw scraped data
├── alikhsancleaned.csv               # Cleaned and processed data
├── README.md                         # Project documentation
└── requirements.txt                  # List of Python libraries used
```

---

## **Setup Instructions**

1. Clone the repository:
   ```bash
   git clone https://github.com/DataEngineering.git
   cd DataEngineering
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the ETL process:
   - Open `Group_assignment_30__SEIS6.ipynb` in Jupyter Notebook.
   - Execute all cells to scrape, clean, and visualize data.

---

## **Tools & Libraries**

- **Libraries**: `BeautifulSoup`, `requests`, `pandas`, `matplotlib`
- **Environment**: Python 3.x, Jupyter Notebook
- **Platform**: Medium for documentation, GitHub for code hosting.

---

## **Key Insights**

- Scraped over **100+ product records** from the Al-Ikhsan website.
- Transformed raw data into a clean format suitable for analysis.
- Visualized key trends in product ratings and discount distribution.

---
