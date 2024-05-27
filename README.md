# SQL_music_store_analysis_Project

# Music Store SQL Analysis

## Overview

This project conducts a comprehensive analysis of a music store database using SQL. By exploring the database schema, querying relevant data, and analyzing sales trends, customer behavior, and inventory management, this analysis aims to provide valuable insights into the operations and performance of the music store.

## Objectives

- Understand sales trends and patterns.
- Analyze customer behavior and preferences.
- Identify popular genres, artists, and albums.
- Provide actionable insights and recommendations for the music store.

## Database Schema

### Structure

The music store database consists of the following tables:

1. **albums**:
   - album_id (Primary Key)
   - title
   - artist_id (Foreign Key referencing artists)
   - ...

2. **artists**:
   - artist_id (Primary Key)
   - name
   - ...

3. **tracks**:
   - track_id (Primary Key)
   - name
   - album_id (Foreign Key referencing albums)
   - ...

4. **customers**:
   - customer_id (Primary Key)
   - first_name
   - last_name
   - ...

5. **invoices**:
   - invoice_id (Primary Key)
   - customer_id (Foreign Key referencing customers)
   - ...

6. **invoice_items**:
   - invoice_line_id (Primary Key)
   - invoice_id (Foreign Key referencing invoices)
   - track_id (Foreign Key referencing tracks)
   - ...

### Relationships

- The `albums` table is related to the `artists` table through the `artist_id` foreign key.
- The `tracks` table is related to the `albums` table through the `album_id` foreign key.
- The `invoices` table is related to the `customers` table through the `customer_id` foreign key.
- The `invoice_items` table is related to the `invoices` table through the `invoice_id` foreign key and to the `tracks` table through the `track_id` foreign key.

## Entity-Relationship Diagram (ER Diagram)

![Database ER Diagram](https://github.com/CodeNinjaSatyam/SQL_music_store_analysis_Project/blob/main/ERD%20music%20database.png)
