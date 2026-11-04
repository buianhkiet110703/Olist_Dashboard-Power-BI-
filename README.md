# End-to-End E-Commerce Data Analytics & Modeling (Olist Dataset)

## 1. Project Context & Dataset Overview
### A. Project Objective
This project aims to build an end-to-end Data Analytics and Engineering portfolio project using the Brazilian E-Commerce Public Dataset by Olist. The primary goal is to transform raw relational CSV files into a structured dimensional model (Star Schema), implement data processing, and design an interactive Power BI dashboard to showcase data modeling and business intelligence skills for a professional CV/GitHub portfolio.
### B. Dataset Description & Table Contents
<img width="2486" height="1496" alt="image" src="https://github.com/user-attachments/assets/507546c9-b17a-453e-b6ea-b0769a69ff0c" />
The dataset comprises 9 core CSV files detailing a multi-seller e-commerce marketplace operation:

-olist_orders_dataset.csv: Contains core order lifecycle metrics, including order status, purchase timestamps, approval dates, carrier delivery dates, actual customer delivery dates, and estimated delivery dates. (Acts as the core event log)

olist_order_items_dataset.csv: Records line-item details for each order, including item sequence ID, product ID, seller ID, shipping limit date, item price, and freight value.

-olist_order_payments_dataset.csv: Captures payment information such as payment sequential, payment type (credit card, boleto, voucher, debit card), number of installments, and payment value.

olist_order_reviews_dataset.csv: Stores customer satisfaction metrics, including review ID, review score (1–5 stars), review comment title, message, creation date, and answer timestamp.

-olist_customers_dataset.csv: Contains customer profile data, including unique customer IDs, customer city, state, and zip code prefixes.

-olist_products_dataset.csv: Details product characteristics, such as category name, name length, description length, photo quantity, weight, and physical dimensions (length, height, width).

-olist_sellers_dataset.csv: Lists third-party marketplace sellers, including seller IDs, cities, states, and zip code prefixes.

-olist_geolocation_dataset.csv: Maps zip code prefixes to geographic coordinates (latitude and longitude), city, and state names for spatial analysis.

-product_category_name_translation.csv: Translates product category names from Portuguese to English for reporting readability.

## 2. Data Modeling in Power BI (Star Schema Architecture)
To optimize query performance, eliminate data redundancy, and ensure seamless DAX measure calculations, the dataset is structured into a classic Star Schema with clearly separated Fact Tables (transactional events) and Dimension Tables (descriptive context).

<img width="1024" height="572" alt="image" src="https://github.com/user-attachments/assets/f6dcf26d-450b-4e3b-96bd-8d649db2aa80" />



