# Key Club Database CLI
<<<<<<< ba4dbed027c6e41a199881df02c0342076c5b10a
<<<<<<< 644c6f7333dfc147ae038bd0c31064a95e60fba0

The North Bergen High School chapter of [Key Club International](https://www.keyclub.org/) needs you to automate
its tracking of student volunteer hours. Additionally, the club needs to submit monthly and annual reports summarizing their service to the community. You will design the database and implement a simple command line interface for adding data and generating reports.

## Database
`keyclub.sqlite` is a [SQLite](https://sqlite.org) database with the following schema:
![keyclub.sqlite schema](img/kc_schema.png)

For clarification, the `officer` field in the `students` table is a boolean. It will hold a 1 if that student is *currently* an officer and a 0 otherwise. This defaults to 0.
<<<<<<< c5307df84935ae56746bdddcc1923d55945faa19

For every school event where Key Club is active, there is always an officer present. Under `events`, the `officer_id` field is the `student_id` of the officer in charge for that event.

## Reports
The database contains the following report views:
### Year-to-date
- `club_ytd`: A view that totals the service hours for the current service year
- `club_month`: A view that totals the service hours for the current month 
- `ind_ytd`: A view that gives the total hours for each member of the club for the current service year
- `officer_ytd`: A view that gives the total hours for each officer in the club for the current service year
- `top_ten`: A view that gives the top ten volunteers and their total service hours for the current service year
### All Time
- `club_all_time`: A view that totals the service hours performed by the club overall
- `ind_all_time`: A view that totals the service hours performed by the club, grouped by student
- `officer_all_time`: A view that totals the service hours performed by the club, grouped by officer
- `top_ten_all_time`: A view that shows the top ten volunteers of all time
=======
>>>>>>> Add title to instructions.md
=======

The North Bergen High School chapter of [Key Club International](https://www.keyclub.org/) needs you to automate
its tracking of student volunteer hours. Additionally, the club needs to submit monthly and annual reports summarizing their service to the community. You will design the database and implement a simple command line interface for adding data and generating reports.

## Database
`keyclub.sqlite` is a [SQLite](https://sqlite.org) database with the following schema:
![keyclub.sqlite schema](img/kc_schema.png)

<<<<<<< a11b85919409397ead611cd8fd39e8be883b121a
Here's the schema for our database:
>>>>>>> Add db schema image into /img folder
=======
For clarification, the `officer` field in the `students` table is in essence a boolean. It will hold a 1 if that student is *currently* an officer and a 0 otherwise. This defaults to 0.
=======
>>>>>>> Add image to instructions.md. Include beginning of reports section

For every school event where Key Club is active, there is always an officer present. Under `events`, the `officer_id` field is the `student_id` of the officer in charge for that event.

## Reports
<<<<<<< HEAD
The administration will need the following reports:
* Total service hours for the current service year
* Total service hours for the current month
>>>>>>> Add image to instructions.md. Include beginning of reports section
=======
The database contains the following report views:
- `club_ytd`: A view that totals the service hours for the current service year
- `club_month`: A view that totals the service hours for the current month 
- `ind_ytd`: A view that gives the total hours for each member of the club for the current service year
- `officer_ytd`: A view that gives the total hours for each officer in the club for the current service year
- `top_ten`: A view that gives the top ten volunteers and their total service hours for the current service year
>>>>>>> 7b38c2858092ca4e0e57d7d46b034f2732fec422
