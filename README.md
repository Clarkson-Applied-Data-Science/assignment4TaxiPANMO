# assignment4TaxiPANMO
 ## Question 1. What datetime range does your data cover?  How many rows are there total?
 ```import csv
from datetime import datetime

# Open the CSV file and read the contents
import csv
import datetime

with open('trip_data_1.csv', 'r') as f:
    reader = csv.reader(f)

    # Get the date range and total number of rows
    dates = []
    row_count = 0
    for row in reader:
        if row_count == 0:
            # Find the index of the column that contains the dates
            date_col_index = row.index('pickup_datetime')

            # Skip the header row
            row_count += 1
            continue

        # Get the date from the specified column of the row
        date_str = row[date_col_index]
        date = datetime.datetime.strptime(date_str, '%Y-%m-%d %H:%M:%S')
        dates.append(date)
        row_count += 1

# Print the date range and total number of rows
print(f"Date range: {min(dates)} to {max(dates)}")
print(f"Total rows: {row_count}")
 ```
