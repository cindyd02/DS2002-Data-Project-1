## DS 2002 Project
# Names: Cindy Dong (ggm7qk) and Carlie Stewart (clstew47)

# Reflection on the ETL Data Processor Project

This project provided us with hands-on experience implementing and understanding key concepts in data science, including SQL, APIs, and flat files, specifically CSV and JSON. Our primary goal was to create a functional and efficient ETL pipeline that can process raw data, limited to JSON or CSV formats, and convert it into one of three output types: SQL, JSON, or CSV.

## Challenges

### Handling Different Data Structures
One of the biggest challenges we faced was managing various data structures and ensuring that the conversion process was adaptable. Parsing and transforming JSON files proved to be particularly difficult, as we worked with nested structures to read in the raw data. We had to research how to flatten JSON files using `json_normalize` from the `pandas` library.

### Add/Remove Column Functionality
Another significant challenge was setting up the add/remove column functionality. Initially, we struggled to implement this interactive feature, which allows users to manually modify columns. We were unsure about which scenarios would require adding columns, but one example we considered was when an individual working with a small dataset might want to insert additional columns to enhance analysis.

To resolve this, we attended office hours for clarification on structuring the feature and verifying its functionality. Our solution involved a `while` loop, where the user can select whether to add or remove columns until they enter 'done' to indicate they are finished with their modifications.

### SQL Integration and Visualization
Integrating the pipeline with SQL and converting a JSON file into a SQL format was also challenging. Since our primary IDE, VSCode, did not allow for direct visualization of the SQL output file, we explored alternatives. This led us to use Tabular, which displays the first five rows of the output database in a table format in the command line.

## What Was Easier than Expected

### Working with CSV Files
Handling CSV files using `pandas` was easier than expected. `pandas`' built-in functions made it simple to manipulate and read CSV files, even for large datasets. The ability to add or remove columns was also straightforward once the pipeline logic was established.

### Data Summaries
Generating summaries of the input and output data was relatively simple. By using `pandas`' descriptive functions, we could easily evaluate CSV and JSON file contents before and after processing through the ETL pipeline.

## Application to Future Projects

Many real-world data tasks involve collecting data from various sources and performing cleaning, transformation, and preparation for analysis. The ability to handle formats like CSV and JSON, modify columns, and store results in databases makes this ETL tool adaptable to a wide range of projects.

For future projects, this tool could be extended to:
- Handle additional file types.
- Scale to accommodate larger datasets.
- Integrate more data cleaning functions.

Overall, this project has strengthened our understanding of ETL processes and data transformation, providing us with practical tools to manage future file transformations effectively.
