# Movies-ETL

Extract, Transform, Load

## Purpose
The purpose of this challenge was to create an ETL pipeline from a raw data format into an SQL database. To do this required python script that would extract data from several different sources. After the data was extracted, it was then cleaned and transform using several different elements of the pandas library. Regular expressions were used to parse data and convert text into numbers. After the data was cleaned and transformed, it was then imported into a PostgreSQL table.



## Extracting
Wikipedia Movies JSON file was extracted first

![1PNG](https://user-images.githubusercontent.com/104540261/182287391-9da9968b-364a-49cf-9cad-66f9844cb1e5.png)

Kaggle Movie Metadata was extracted second

![2PNG](https://user-images.githubusercontent.com/104540261/182287431-127d94a1-beae-45c4-a06e-e2ca81daefd4.png)

Kaggle Ratings data was extracted third

![3PNG](https://user-images.githubusercontent.com/104540261/182287506-f0dc2c3e-8118-472a-abb3-21ba187001bc.png)


## Transforming 
### Wikipedia Data
Wikipedia Movies transformed

![4PNG](https://user-images.githubusercontent.com/104540261/182287539-2e4fb518-0b00-4816-a18f-11808731fea8.png)


Wikipedia Movies was converted into a cleaner format

![5PNG](https://user-images.githubusercontent.com/104540261/182287573-c500026d-20d3-4d69-9b30-a18ef0172578.png)

### Kaggle Data
Wikipedia Movies were merged with Kaggle Movies data


![6PNG](https://user-images.githubusercontent.com/104540261/182287656-57d4d6f3-47a4-4b27-9bbb-a4b3ca426706.png)

Movies and kaggle ratings were merged together


![7PNG](https://user-images.githubusercontent.com/104540261/182287809-6fb6d344-e212-4f0d-a06c-39f986f15aa1.png)

## Loading
### Creating the Movie Database

Importing the data to the movies database

![8PNG](https://user-images.githubusercontent.com/104540261/182287951-2cd1e424-44de-435b-bf22-637f340317e1.png)


### Verifying the data in PgAdmin
Movies Query

![movies_query](https://user-images.githubusercontent.com/104540261/182288002-a5b87cf1-9a35-4f13-a61c-157af90dd60e.png)


Ratings Query


![ratings_query](https://user-images.githubusercontent.com/104540261/182288038-cab68d0a-5d07-4e66-b225-ed38c6072b24.png)

## Summary

The hack-a-thon event was complete upon loading the movies and ratings data into tables in the movies database. The data that was extracted, transformed, and loaded was comprised of a JSON file and 2 Kaggle files.
