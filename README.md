# Azure-SQL-MichiganX-Introduction-to-Data-Analytics-for-Managers

## Overview:

This repo is to store notes from the cours of MichiganX using Azure and SQL

## Languages and Tools:

- Microsoft Azure Machine Learning Studio

- Azure

- SQL

## Data Analysis:

```
select movie_title
from t1
where title_year = 2016;
```
![Basic Sql](https://user-images.githubusercontent.com/70437668/154830738-e8f465a6-0229-46c0-b876-263eaa157a55.jpg)

```
select avg(gross), avg(imdb_score)
from t1
where title_year = 2016
and gross > 0;
```

![avg](https://user-images.githubusercontent.com/70437668/154830740-5e0259fc-b331-4649-828b-47660c400ade.jpg)

```
select distinct movie_title, gross, imdb_score
from t1
where title_year = 2016
and genres like "%Comedy%";
```

![comedy](https://user-images.githubusercontent.com/70437668/154830743-d2c561ee-ad22-4559-be64-9fef3f4a9760.jpg)

```
select distinct movie_title, gross, imdb_score
from t1
where title_year = 2016
and genres like "%!Comedy%";
```
![not comedy](https://user-images.githubusercontent.com/70437668/154830749-370358b8-d5da-463b-b80f-6ccf5c4cc3c8.jpg)

```
select title_year, avg(gross)
from t1
group by title_year;
```
![group by year](https://user-images.githubusercontent.com/70437668/154830752-fadeadd8-cd20-415a-93b7-39e173869327.jpg)

```
select title_year, content_rating, avg(gross)
from t1
where title_year >= 2000
group by title_year, content_rating;
```

![group by year, content rating](https://user-images.githubusercontent.com/70437668/154830753-5869fc6a-f9ab-404c-a2f7-6f411943d27c.jpg)

![Import academy](https://user-images.githubusercontent.com/70437668/154830760-556a6bb7-53dc-40cb-b075-c2a23fb87236.jpg)

![join](https://user-images.githubusercontent.com/70437668/154830761-73b7d33d-900d-4a54-90fd-0be1b55f7b78.jpg)

![year correct, winners](https://user-images.githubusercontent.com/70437668/154830765-9c2b42ed-5ec2-4838-9b1d-3d67a759d473.jpg)

### Credit Card dataset:

#### Overview:

![Credit Card dataset nuggets](https://user-images.githubusercontent.com/70437668/154832386-ca37a3df-6f25-4fce-a54b-3849976aa8e8.jpg)

##### High School:

![High School](https://user-images.githubusercontent.com/70437668/154832075-6d26761c-f264-49bd-9cd0-8e2ea53b94f5.jpg)

![High School 2](https://user-images.githubusercontent.com/70437668/154832076-140ed7df-a527-453d-a763-884d2cc40b6a.jpg)

![High School dot plot](https://user-images.githubusercontent.com/70437668/154832371-2f72273a-6785-4327-9056-79361fd89770.jpg)

![High School corr](https://user-images.githubusercontent.com/70437668/154832392-7743204b-cd8d-4a34-875e-ddde38eb3c62.jpg)

##### Masters:

![Masters ](https://user-images.githubusercontent.com/70437668/154832372-1c27491c-180a-484c-a8cd-24ae7a681121.jpg)

![Masters 2](https://user-images.githubusercontent.com/70437668/154832375-16ba96e4-2d99-4641-acbf-8030b8e79de3.jpg)

![Masters dot plot](https://user-images.githubusercontent.com/70437668/154832382-25b04989-8971-41b9-adf1-283d488c96e7.jpg)

![Masters corr](https://user-images.githubusercontent.com/70437668/154832393-59b23e12-d803-42bf-a39d-e3720576f4dc.jpg)

## Descriptive 

Standard reports are reports that are either constantly evaluated, or with very regular periodicity. Let's say, every quarter, or every week, or every month. So that a bunch of KPIs that you're looking at, let's say every month. You're looking at your sales every month. And you're looking at your cost of goods sold, or your sales and administrative expenses, every month. That is what we'd call a standard report.

There are ad hoc reports. This is descriptive data collected on a one time, or a special case basis. So that you can understand something in the moment. A special project that you're doing to try and, let's say, launch a new product. That may require one or more ad hoc reports. And so, here you see an example of a dashboard, that has many of these things already inside it, right? You have your visuals and your quants. You have your standard reports, such as the budget and the finance marketing sales. The expenses by different categories, and so on. You also have the ability to drill down. Drill down is the idea that you go deeper into some specific aspects, or pieces, of your data.


