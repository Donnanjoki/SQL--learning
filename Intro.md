Source: https://www.sqlstyle.guide/

### GENERAL SPECIFICATIONS

PART A: TO DO's

1. Use consistent and descriptive identifiers and names.

2. Utilize white space and indentation to make code easier to read.

3. Store ISO 8601 compliant time and date information (YYYY-MM-DD HH:MM:SS.SSSSS).

4. Only use standard SQL function of vendor-specific functions for reasons of portability.

5. Keep code succinct and devoid of redundant SQL - this might be inclusive of unnecessary quoting or parentheses or WHERE clauses which can be otherwise derived.

6. Include comments in SQL code where necessary

//Example:

# updating the file record after writing to the file

UPDATE file_system
SET file_modified_date = '1980-02-22 13:19:01.00000',
file_size = 209732
WHERE file_name = '.vimrc';

PART B - AVOID

1. CamelCase as it is difficult to scan quickly.

2. Descriptive prefixes or hungarian notation such as sp\_ or tbl.

3. Plurals - use more natural collective term instead; e.g. staff rather than employees || people instead individuals.

4. Quoted identifiers - if you must use them then stick to SQL-92 double quotes for portability (you may need to configure your SQL server to support this depending on vendor).

5. Object-oriented design principles should not be applied to SQL or database structures.

### NAMING CONVENTIONS

# General::

1. Ensure the name is unique and does not exist as a reserved keyword.

2. Keep the length to a maximum of 30 bytes - that is 30 characters unless using a multi-byte character set.

3. Names must begin with a letter and may not end with an underscore.

4. Only use letters, numbers and underscores in names.

5. Avoid the use of multiple consecutive underscore, as they can be hard to read.

6. Use underscores where you would naturally include a space in the name (e.g. first_name)

7. Avoid abbreviations and if you have to use them make sure they are commonly understood.

# Tables::

A. Use a collective name, less ideally, a plural form.

B. Do not prefix tbl or any other such descriptive prefix or hungarian notation.

C. Never give a table the same name as of of its column or vice versa

D. Avoid, where possible, concatenating two table names together to create the name of a relationship table. e.g rather than cars_mechanics use instead services.

# Columns::

# Aliasing or correlations::

# Stored procedures

# Uniform suffixes::

### QUERY SYNTAX
