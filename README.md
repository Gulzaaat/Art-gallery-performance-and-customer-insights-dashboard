### **Power BI Dashboard for Art Gallery - Overview**

This dashboard visualizes and analyzes data related to an art gallery, focusing on exhibitions, artworks, artists, transactions, and customers. It provides insights into artwork mediums, exhibition statistics, customer demographics, and transactions.

#### **Key Features and Data Structure:**

1. **Star Schema Data Model**:

   * The **public artists** table connects to **public artworks** through `artist_id`.
   * **Public transactions** are linked to **public artworks** by `artwork_id` to analyze sales.
   * **Public exhibition_artworks** connects artworks to exhibitions through `artwork_id` and `exhibition_id`.
   * The **Calendar** table is integrated with transaction dates for time-based analysis (e.g., monthly, yearly).
   * **Public exhibitions** and **public rents** link through `exhibition_id` and `head_id`, enabling detailed event and customer data analysis.

2. **Interactive Visuals**:

   * **City-wise Data**: Shows the number of exhibitions across different cities, enabling geographic analysis.
   * **Artwork Analysis**: Displays artwork mediums and their sales performance, highlighting popular art forms (e.g., oil on canvas).
   * **Customer & Artist Details**: Provides a detailed view of artists’ nationalities, names, and customer interactions.
   * **Exhibition & Transaction Insights**: Shows the number of artworks, total sales, and top artists, helping users understand the gallery's overall performance.

#### **Power BI Features**:

* **Q&A**: Allows users to ask questions about the data (e.g., “Top media by max income” or “Top media by anniversary”).
* **Charts and Graphs**: Includes bar and pie charts for artwork distribution, customer demographics, and VIP clients.
* **Time Intelligence**: Utilizes the **Calendar** table to show sales and artworks over time, including trends in artwork quantity and revenue.


## Key insights:
- Artworks & Sales performance: The dashboard provides clear insights into which artworks, mediums, and artists are generating the most sales, allowing the gallery to focus on high-performing items and artists.
- Customer segmentation: The data reveals customer demographics and purchasing patterns, enabling the gallery to better target its marketing and customer engagement strategies.
- Exhibition effectiveness: By analyzing exhibition data, the dashboard highlights which events are the most successful, helping to optimize future exhibitions and planning.
- Time-based analysis: The time intelligence features offer a clear view of sales trends and performance over time, enabling the gallery to predict future sales cycles and adjust strategies accordingly.
