# Data-Analysis---Project---Uber-Drives

kaggle dataset = my uber drives

Answer the below questions:
1.	Get the unique start and stop location
2.	What are the most famous start and stop location
3.	Highest average speed  by purpose
4.	Highest average speed by category

Steps to follow:

•	First, we should clean our data
•	Start and end date are in date time format and some of the row are in different format
•	Split the date time into 2 columns as start date and start time as well as for end date time.
•	Make all date in dd-mm-yyyy and time in hh.mm.ss (24 hr) format
•	Find time difference, end time – start time * 24 * 60, to find difference in hour divide it by 60
•	Then, to find speed, speed = miles/time.
•	There is a problem in above approach, if start and end dates differs, it gives negative values. It it wrong.
•	To avoid that convert the time format to 12 hour format
•	In time difference put if condition(end time> start time, end time-start time, end time-start time+1)
•	Then calculate hour using formula =(HOUR(time diff.)*60+MINUTE (time diff.))/60
•	Calculate speed
•	Div!/0 error in speed appears in some rows, incorrect data, delete those rows
•	There is some abnormal speed ranges, check the speed limits.
•	Use outliner concept for optimum ranges
•	Here, I deleted the values above speed 160 mph.
•	Data cleaning finished
•	Analyse data for mentioned questions

