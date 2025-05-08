# 🎬 Movie Analytics Dataset

This is a relational database project consisting of 5 interconnected tables that capture comprehensive data about movies, including their language, actor, financial, movie actor.

---

## 🎯 Objective

The goal of this dataset project is to provide a structured and relational view of movie data that spans multiple film industries, languages, and  ratings. By organizing the data into five interrelated tables, this dataset enables:

- 📊 In-depth analysis of movie trends by year, industry, and studio  
- 🌐 Multilingual and cross-industry comparisons  
- 🏆 Identification of top- and bottom-rated movies using IMDb scores  
- 🤖 Applications in machine learning (e.g., rating prediction, clustering)  
- 📚 Practice for SQL queries and relational database design  
---

## 🗂️ Dataset Structure

The dataset consists of 5 tables:

1. `movies`
2. `languages`
3. `movie_actor`
4. `financials`
5. `actors`

Each table is explained below with its purpose and key fields.

---

## 🧾 Table Descriptions

### 1. `movies`
Stores core details about each movie.

| Column Name   | Data Type | Description                              |
|---------------|-----------|------------------------------------------|
| movie_id      | INT       | Primary Key - Unique ID for each movie   |
| title         | VARCHAR   | Movie title                              |
| industry   | INT       | Foreign Key → `industries.industry_id`   |
| release_year  | YEAR      | Year of release                          |
| studio    | INT       | Foreign Key → `studios.studio_id`        |
| release_year   | INT       | Foreign Key → `languages.language_id`    |

---

### 2. `languages`
Lists all supported languages.

| Column Name   | Data Type | Description              |
|---------------|-----------|--------------------------|
| language_id   | INT       | Primary Key              |
| name | VARCHAR   | Name of the language     |

---

### 3. `movie_actor`
Contains studio or production company information.

| Column Name   | Data Type | Description                  |
|---------------|-----------|------------------------------|
|   actor_id     | INT       | Primary Key                  |
|  movie_id| INT   | Name of the studio           |

---

### 4. `financials`
Holds IMDb rating information for movies.

| Column Name   | Data Type | Description                              |
|---------------|-----------|------------------------------------------|
| movie_id     | INT       | Primary Key                              |
| budget      | DECIMAL       | BUDGET OF MOVIE          |
| revenue   | DECIMAL   |      REVENUE GENEATED BY MOVIE                  |
| unit   | VARCHAR   |                         |
| currency   | VARCHAR   |    CURRENCY                     |

---

### 5. `actors`
Defines the film industries (e.g., Bollywood, Hollywood).

| Column Name     | Data Type | Description             |
|------------------|-----------|-------------------------|
| actor_id      | INT       | Primary Key             |
| name    | VARCHAR   | Name ACTOR    |
| birth_year    | DATE   | BIRTH YEAR    |
---

## 💡 Example Use Cases

- Get the top 10 highest-rated movies in Hollywood  
- Find average ratings of movies by language  
- Join `movies`, `studios`, and `ratings` to analyze performance by production house  
- Identify underperforming movies for a particular year  
- Use for SQL practice projects or database schema design assignments  

---

## 🛠️ Technologies Used

- 🐘 MySQL
- 📊 SQL for queries  
- 📄 Markdown for documentation  
- 🔄 Relational Database Concepts  

---


