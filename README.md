# 🎬 Movie Analytics Dataset

This is a relational database project consisting of 5 interconnected tables that capture comprehensive data about movies, including their language, studio, industry, and IMDb ratings. It is useful for practicing SQL queries, relational joins, and performing data analysis or machine learning tasks on real-world structured data.

---

## 🎯 Objective

The goal of this dataset project is to provide a structured and relational view of movie data that spans multiple film industries, studios, languages, and user ratings. By organizing the data into five interrelated tables, this dataset enables:

- 📊 In-depth analysis of movie trends by year, industry, and studio  
- 🌐 Multilingual and cross-industry comparisons  
- 🏆 Identification of top- and bottom-rated movies using IMDb scores  
- 🤖 Applications in machine learning (e.g., rating prediction, clustering)  
- 📚 Practice for SQL queries and relational database design  

This dataset is ideal for developers, analysts, and students interested in exploring real-world SQL operations, data modeling, and entertainment data insights.

---

## 🗂️ Dataset Structure

The dataset consists of 5 tables:

1. `movies`
2. `languages`
3. `studios`
4. `ratings`
5. `industries`

Each table is explained below with its purpose and key fields.

---

## 🧾 Table Descriptions

### 1. `movies`
Stores core details about each movie.

| Column Name   | Data Type | Description                              |
|---------------|-----------|------------------------------------------|
| movie_id      | INT       | Primary Key - Unique ID for each movie   |
| title         | VARCHAR   | Movie title                              |
| industry_id   | INT       | Foreign Key → `industries.industry_id`   |
| release_year  | YEAR      | Year of release                          |
| studio_id     | INT       | Foreign Key → `studios.studio_id`        |
| language_id   | INT       | Foreign Key → `languages.language_id`    |

---

### 2. `languages`
Lists all supported languages.

| Column Name   | Data Type | Description              |
|---------------|-----------|--------------------------|
| language_id   | INT       | Primary Key              |
| language_name | VARCHAR   | Name of the language     |

---

### 3. `studios`
Contains studio or production company information.

| Column Name   | Data Type | Description                  |
|---------------|-----------|------------------------------|
| studio_id     | INT       | Primary Key                  |
| studio_name   | VARCHAR   | Name of the studio           |

---

### 4. `ratings`
Holds IMDb rating information for movies.

| Column Name   | Data Type | Description                              |
|---------------|-----------|------------------------------------------|
| rating_id     | INT       | Primary Key                              |
| movie_id      | INT       | Foreign Key → `movies.movie_id`          |
| imdb_rating   | DECIMAL   | IMDb rating score                        |

---

### 5. `industries`
Defines the film industries (e.g., Bollywood, Hollywood).

| Column Name     | Data Type | Description             |
|------------------|-----------|-------------------------|
| industry_id      | INT       | Primary Key             |
| industry_name    | VARCHAR   | Name of the industry    |

---

## 💡 Example Use Cases

- Get the top 10 highest-rated movies in Hollywood  
- Find average ratings of movies by language  
- Join `movies`, `studios`, and `ratings` to analyze performance by production house  
- Identify underperforming movies for a particular year  
- Use for SQL practice projects or database schema design assignments  

---

## 🛠️ Technologies Used

- 🐘 MySQL / PostgreSQL  
- 📊 SQL for queries  
- 📄 Markdown for documentation  
- 🔄 Relational Database Concepts  

---

## 📁 How to Use

1. Clone the repository  
   ```bash
   git clone https://github.com/your-username/movie-analytics-dataset.git
