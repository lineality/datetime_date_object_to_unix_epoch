# datetime_date_object_to_unix_epoch
convert a datetime.date object into epoch time

Python3 code
```
# Convert a datetime.date object to a datetime.datetime object

from datetime import date, datetime

just_a_date = date.today()

# inspection
print(just_a_date)

converted_to_datetime = datetime.combine( just_a_date, datetime.min.time())
# inspection
print(converted_to_datetime)

unix_time = datetime.timestamp(converted_to_datetime)  # *1000
print(unix_time)
```
