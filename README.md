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
| industry   | INT       | Type of industry   |
| release_year  | YEAR      | Year of release                          |
| studio    | INT       | Under which studio released`        |
| release_year   | INT       | Release year    |

---

### 2. `languages`
Lists all supported languages.

| Column Name   | Data Type | Description              |
|---------------|-----------|--------------------------|
| language_id   | INT       | Primary Key              |
| name | VARCHAR   | Name of the language     |

---

### 3. `movie_actor`
Contains movie actor information

| Column Name   | Data Type | Description                  |
|---------------|-----------|------------------------------|
|   actor_id     | INT       | Primary Key                  |
|  movie_id| INT   | Id of Movie          |

---

### 4. `financials`
Holds financials information for movies.

| Column Name   | Data Type | Description                              |
|---------------|-----------|------------------------------------------|
| movie_id     | INT       | Primary Key                              |
| budget      | DECIMAL       | Budegt of movie        |
| revenue   | DECIMAL   |      Revenue of movie                 |
| unit   | VARCHAR   |                  Unit of currency       |
| currency   | VARCHAR   |    Currency                  |

---

### 5. `actors`
Contains actors name and their information

| Column Name     | Data Type | Description             |
|------------------|-----------|-------------------------|
| actor_id      | INT       | Primary Key             |
| name    | VARCHAR   | Actor Name   |
| birth_year    | DATE   | Birth Year    |
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


