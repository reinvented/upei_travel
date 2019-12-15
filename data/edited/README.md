After combining the raw CSV files received from my FOIPP request:

	cat * > ../combined/upei-travel-201904-201910.csv

I removed the duplicate header lines, and then made the following edits:

1. Removed all leading dollar signs ($) from cost figures.
2. Removed the words "night" and "nights" from the duration field.
3. Removed the words "day" and "days" from the duration field.
4. Removed the dash from missing fields.
5. Added a new "Total Cost" column that combines transportation and lodging.
6. Normalized names that had multiple variations ("Doug" and "Douglas," for example).
7. Removed the empty third column.
8. Normalized the "Purpose" column ("Meetings" to "Meeting," etc.)
9. Normalized the "Faculty/Department" column.

The result is [upei-travel-201904-201910-with-total.csv](upei-travel-201904-201910-with-total.csv).
