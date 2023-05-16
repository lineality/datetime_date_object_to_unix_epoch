# datetime_date_object_to_unix_epoch
convert a datetime.date object into epoch time


Readable String Timestamp
```
# # Make a timestamp

import datetime, calendar, time
from datetime import date, datetime

# get time
Sample_Time = datetime.utcnow()

# make readable string
readable_string_timestamp = Sample_Time.strftime('v_%Y_%m_%d__%H%M_%S')

readable_string_timestamp = str(readable_string_timestamp)

# inspection
print(readable_string_timestamp)
```

Python3 code
```
# Convert a datetime.date object to a datetime.datetime object

from datetime import date, datetime

# your date time object would be here
just_a_date = date.today()

# inspection
print(just_a_date)

converted_to_datetime = datetime.combine( just_a_date, datetime.min.time())
# inspection
print(converted_to_datetime)

unix_time = datetime.timestamp(converted_to_datetime)  # *1000
print(unix_time)
```
