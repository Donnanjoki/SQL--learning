Source: https://www.sqlstyle.guide/

GENERAL SPECIFICATIONS

1. Use consistent and descriptive identifiers and names.

2. Utilize white space and indentation to make code easier to read.

3. Store ISO 8601 compliant time and date information (YYYY-MM-DD HH:MM:SS.SSSSS).

4. Only use standard SQL function of vendor-specific functions for reasons of portability.

5. Keep code succinct and devoid of redundant SQL - this might be inclusive of unnecessary quoting or parentheses or WHERE clauses which can be otherwise derived.

6. Include comments in SQL code where necessary

//Example:

## updating the file record after writing to the file

UPDATE file_system
SET file_modified_date = '1980-02-22 13:19:01.00000',
file_size = 209732
WHERE file_name = '.vimrc';
