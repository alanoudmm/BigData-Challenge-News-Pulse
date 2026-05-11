# SE446 BigData Challenge News Pulse

## Project Overview

News Pulse is a simplified real-time big-data processing pipeline developed using Python and PySpark. The project demonstrates the core concepts of data ingestion, simulated streaming, data processing, aggregation, and real-time output visualization within a lightweight academic environment.

The system processes news headline records from a CSV dataset and performs different transformations and analytics using PySpark DataFrames.

---

# Student Name & ID

- Alanoud Almeniya — 231385

---


# Features Implemented

## 1. Data Ingestion
The system reads structured news headline records from a CSV dataset containing:
- timestamp
- source
- headline

---

## 2. Simulated Streaming Processing
Instead of production-level real-time streaming, the project uses simulated streaming batches through a loop with time intervals.

This continuously processes incoming data batches and mimics real-time behavior.

---

## 3. Data Processing and Aggregation

The pipeline performs several transformations including:

### Headlines by Source
Counts how many headlines are published by each news source.

### Trending Keywords
Extracts individual words from headlines and counts keyword frequency to identify trending topics.

### Simple Statistics
Calculates the total number of processed headlines.

---

## 4. Output Visualization

Results are displayed dynamically in console tables using PySpark `.show()` output.

Example outputs include:
- source-wise headline counts
- trending keywords
- total processed records

---

# Dataset Information

The dataset contains:
- 100 news headline records
- multiple international news sources
- timestamps and headline text

---

# Program Output

```text
News Pulse Streaming Started...

===== Headlines By Source =====
+------------+-----+
|source      |count|
+------------+-----+
|Bloomberg   |12   |
|NBC News    |13   |
|Al Jazeera  |13   |
|Reuters     |12   |
|Fox News    |13   |
|CNN         |12   |
|The Guardian|13   |
|BBC         |12   |
+------------+-----+


===== Trending Keywords =====
+-------------+-----+
|word         |count|
+-------------+-----+
|online       |4    |
|launch       |3    |
|International|7    |
|battery      |3    |
|renewable    |3    |
|Education    |3    |
|space        |3    |
|experts      |6    |
|markets      |3    |
|industry     |6    |
|Cybersecurity|3    |
|Clean        |3    |
|prices       |4    |
|demand       |4    |
|launches     |4    |
|companies    |3    |
|attract      |6    |
|new          |9    |
|Banks        |3    |
|investors    |3    |
+-------------+-----+
only showing top 20 rows

Total Headlines Processed: 100

Waiting for next streaming batch...


===== Headlines By Source =====
+------------+-----+
|source      |count|
+------------+-----+
|Bloomberg   |12   |
|NBC News    |13   |
|Al Jazeera  |13   |
|Reuters     |12   |
|Fox News    |13   |
|CNN         |12   |
|The Guardian|13   |
|BBC         |12   |
+------------+-----+


===== Trending Keywords =====
+-------------+-----+
|word         |count|
+-------------+-----+
|online       |4    |
|launch       |3    |
|International|7    |
|battery      |3    |
|renewable    |3    |
|Education    |3    |
|space        |3    |
|experts      |6    |
|markets      |3    |
|industry     |6    |
|Cybersecurity|3    |
|Clean        |3    |
|prices       |4    |
|demand       |4    |
|launches     |4    |
|companies    |3    |
|attract      |6    |
|new          |9    |
|Banks        |3    |
|investors    |3    |
+-------------+-----+
only showing top 20 rows

Total Headlines Processed: 100

Waiting for next streaming batch...


===== Headlines By Source =====
+------------+-----+
|source      |count|
+------------+-----+
|Bloomberg   |12   |
|NBC News    |13   |
|Al Jazeera  |13   |
|Reuters     |12   |
|Fox News    |13   |
|CNN         |12   |
|The Guardian|13   |
|BBC         |12   |
+------------+-----+


===== Trending Keywords =====
+-------------+-----+
|word         |count|
+-------------+-----+
|online       |4    |
|launch       |3    |
|International|7    |
|battery      |3    |
|renewable    |3    |
|Education    |3    |
|space        |3    |
|experts      |6    |
|markets      |3    |
|industry     |6    |
|Cybersecurity|3    |
|Clean        |3    |
|prices       |4    |
|demand       |4    |
|launches     |4    |
|companies    |3    |
|attract      |6    |
|new          |9    |
|Banks        |3    |
|investors    |3    |
+-------------+-----+
only showing top 20 rows

Total Headlines Processed: 100

Waiting for next streaming batch...


===== Headlines By Source =====
+------------+-----+
|source      |count|
+------------+-----+
|Bloomberg   |12   |
|NBC News    |13   |
|Al Jazeera  |13   |
|Reuters     |12   |
|Fox News    |13   |
|CNN         |12   |
|The Guardian|13   |
|BBC         |12   |
+------------+-----+


===== Trending Keywords =====
+-------------+-----+
|word         |count|
+-------------+-----+
|online       |4    |
|launch       |3    |
|International|7    |
|battery      |3    |
|renewable    |3    |
|Education    |3    |
|space        |3    |
|experts      |6    |
|markets      |3    |
|industry     |6    |
|Cybersecurity|3    |
|Clean        |3    |
|prices       |4    |
|demand       |4    |
|launches     |4    |
|companies    |3    |
|attract      |6    |
|new          |9    |
|Banks        |3    |
|investors    |3    |
+-------------+-----+
only showing top 20 rows

Total Headlines Processed: 100

Waiting for next streaming batch...


===== Headlines By Source =====
+------------+-----+
|source      |count|
+------------+-----+
|Bloomberg   |12   |
|NBC News    |13   |
|Al Jazeera  |13   |
|Reuters     |12   |
|Fox News    |13   |
|CNN         |12   |
|The Guardian|13   |
|BBC         |12   |
+------------+-----+


===== Trending Keywords =====
+-------------+-----+
|word         |count|
+-------------+-----+
|online       |4    |
|launch       |3    |
|International|7    |
|battery      |3    |
|renewable    |3    |
|Education    |3    |
|space        |3    |
|experts      |6    |
|markets      |3    |
|industry     |6    |
|Cybersecurity|3    |
|Clean        |3    |
|prices       |4    |
|demand       |4    |
|launches     |4    |
|companies    |3    |
|attract      |6    |
|new          |9    |
|Banks        |3    |
|investors    |3    |
+-------------+-----+
only showing top 20 rows

Total Headlines Processed: 100

Waiting for next streaming batch...

Streaming Finished.
```
