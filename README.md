# Movies-ETL

Extract, Transform, Load

## Purpose
1. Create an ETL pipeline from raw data to a SQL database.
2. Extract data from disparate sources using Python.
3. Clean and transform data using Pandas.
4. Use regular expressions (Regex) to parse data and to transform text into numbers.
5. Load data with PostgreSQL and verify in PgAdmin.

The project included extracting a large data set from Kaggle, then transforming the data into a usable dataset for a "hacking competition."  Once the data was transformed and narrowed in scope for the hack-a-thon, the DataFrames were loaded into PostgresSQL.  

## Extracting
Wikipedia Movies JSON file, starting with 193 Columns:

![1PNG](https://user-images.githubusercontent.com/104540261/182287391-9da9968b-364a-49cf-9cad-66f9844cb1e5.png)

Kaggle Movie Metadata, 24 columns

![2PNG](https://user-images.githubusercontent.com/104540261/182287431-127d94a1-beae-45c4-a06e-e2ca81daefd4.png)

Kaggle Ratings data, 2602489 rows by 4 columns

![3PNG](https://user-images.githubusercontent.com/104540261/182287506-f0dc2c3e-8118-472a-abb3-21ba187001bc.png)


## Transforming 
### Wikipedia Data
Wikipedia Movies transformed, 22 columns

![4PNG](https://user-images.githubusercontent.com/104540261/182287539-2e4fb518-0b00-4816-a18f-11808731fea8.png)


Wikipedia Movies, making the column names more succinct and uniform, 7033 rows of data.

![5PNG](https://user-images.githubusercontent.com/104540261/182287573-c500026d-20d3-4d69-9b30-a18ef0172578.png)

### Kaggle Data
Wikipedia Movies merged with Kaggle Movies data, all column names and row counts, 6052 rows.


![6PNG](https://user-images.githubusercontent.com/104540261/182287656-57d4d6f3-47a4-4b27-9bbb-a4b3ca426706.png)

Merged Movies with Kaggle ratings, all of the column names and row counts, 6052 rows.


![7PNG](https://user-images.githubusercontent.com/104540261/182287809-6fb6d344-e212-4f0d-a06c-39f986f15aa1.png)

## Loading
### Creating the Movie Database
Sending the data to PostgresSQL

![8PNG](https://user-images.githubusercontent.com/104540261/182287951-2cd1e424-44de-435b-bf22-637f340317e1.png)


### Verifying the data in PgAdmin
Movies Query

![movies_query](https://user-images.githubusercontent.com/104540261/182288002-a5b87cf1-9a35-4f13-a61c-157af90dd60e.png)


Ratings Query


![ratings_query](https://user-images.githubusercontent.com/104540261/182288038-cab68d0a-5d07-4e66-b225-ed38c6072b24.png)

## Summary

A JSON file and 2 Kaggle files were extracted, then transformed, and joined.  A movies and ratings file were loaded into a database for the hack-a-thon event.
