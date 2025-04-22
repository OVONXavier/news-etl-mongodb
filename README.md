# news-etl-mongodb
A lightweight, modular ETL (Extract–Transform–Load) pipeline built in Python to extract news articles from the NewsData.io public API, transform them into clean CSV format, and load them into a MongoDB Atlas cloud database.


# 📰 News ETL Pipeline with MongoDB Atlas

A lightweight, modular ETL (Extract–Transform–Load) pipeline built in Python to extract news articles from the [NewsData.io](https://newsdata.io/documentation) public API, transform them into clean CSV format, and load them into a MongoDB Atlas cloud database.

## 📌 Features

- ✅ Extracts news articles on **Artificial Intelligence**, **LLMs**, and **Robotics**
- ✅ Cleans and stores data in a structured **CSV file**
- ✅ Uploads data into a **MongoDB Atlas** cloud collection
- ✅ Handles basic error detection and retries
- ✅ Well-documented Jupyter Notebook

---

## 🛠️ Technologies Used

- Python 3.8+
- [`requests`](https://pypi.org/project/requests/)
- [`pymongo`](https://pypi.org/project/pymongo/)
- [`csv`](https://docs.python.org/3/library/csv.html)
- MongoDB Atlas (Cloud)
- Jupyter Notebook

---

## 🧠 Workflow Overview

1. **Extract**: Connects to NewsData.io API and fetches real-time news based on specific keywords.
2. **Transform**: Normalizes the JSON response and converts it to structured CSV format.
3. **Load**: Pushes the records to a MongoDB Atlas database collection.

---

## 📂 Project Structure

```bash
📁 news-etl-mongodb/
├── webscrape_and_mongdb.ipynb   # Jupyter Notebook with full ETL code
├── requirements.txt             # Python dependencies
├── README.md                    # Project documentation (this file)
├── output/
│   └── news_api_us.csv          # Extracted and cleaned data
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/news-etl-mongodb.git
cd news-etl-mongodb
```

### 2. Set up the environment

Install the required libraries:

```bash
pip install -r requirements.txt
```

### 3. Add your credentials

Edit the `webscrape_and_mongdb.ipynb` file to:

- Replace `API_key` with your own from [NewsData.io](https://newsdata.io/register).
- Replace the MongoDB connection URI with your secure Atlas string.

### 4. Run the ETL pipeline

Open the notebook and run all cells to:

- Pull news data
- Save it as CSV
- Upload to MongoDB Atlas

---

## 🛡️ Security Tip

⚠️ Never commit your MongoDB URI or API keys directly into public repos. Use `.env` and `python-dotenv` for secret management.

---

## 📊 Example Output

- MongoDB Collection: `news_data_api.The_articles`
- Sample Document:
```json
{
  "article_id": "123456",
  "title": "AI Revolution in Healthcare",
  "link": "https://example.com/ai-healthcare",
  "source_name": "TechCrunch",
  "pubDate": "2025-04-22",
  "country": "US",
  "category": "Technology"
}
```

---

## 📚 References

- [NewsData.io API Docs](https://newsdata.io/documentation)
- [MongoDB Atlas Quickstart](https://www.mongodb.com/developer/products/atlas/)
- [Python for Data Analysis – Wes McKinney](https://wesmckinney.com/book/)

---

## 🙌 Author

**[Francis Xavier OVON]** – MSc Computer Science, Muni University  
📫 Reach me at: [foxnesta.vfx58@gmail.com]
