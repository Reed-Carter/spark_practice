# spark_practice

#### By [Reed Carter](https://github.com/Reed-Carter)

#### This repo is a code review to demonstrate an understanding of spark 

<br>

## Technologies Used

* Spark
* Python
* Git
* Markdown
  
</br>

## Assignment:

Set Up the Data
1. Read the coffee data CSV file into a Spark DataFrame.

Columns from Aggregate Functions
1. Add a column to the DataFrame where the values are the difference between 'Open' and 'Close'.

2. Add a column to the DataFrame where the values are the difference between 'High' and 'Low'.

3. Add a column to the DataFrame where the values are 'True' if the volume for that day was 100 or above, and otherwise 'False'.

4. Once you have a column for the difference between 'Open' and 'Close', add another column that contains the absolute values of the numbers in that column.

5. Compute a column called net_sales which is the average of opening, high, low, and closing cost times the volume: net_sales = avg(opening, high, low, closing price) * volume

Stats
1. Find the average of the values in the column that has the absolute values of the difference between 'Open' and 'Close'.

2. Get the count of values where the 'Volume' was less than 100.

3. Find the average 'Open' value.

4. Get the highest 'High' value.

Write File
1. Save your DataFrame (including the four added columns) to /data as a parquet file.


## Setup/Installation Requirements

* Go to https://github.com/Reed-Carter/spark_practice to find the specific repository for this website.

* Then clone the repository by inputting: 
  ```bash
  git clone https://github.com/Reed-Carter/spark_practice
  ```
* Go into the new directory:
  ```bash
  cd Airflow-Practice
  ```
* Once in the directory you will need to set up a virtual environment in your terminal:
  ```bash
  python3.7 -m venv venv
  ```
* Then activate the environment:
  ```bash
  source venv/bin/activate
  ```
* Install the necessary items with requirements.txt:
  ```bash
    pip install -r requirements.txt

* Download the coffee.csv data file:
  ``` bash
  gsutil -m cp gs://data.datastack.academy/coffee_price/coffee.csv ./data/
  ```
* open your code editor and run all the notebook clls in main.ipynb:
  ``` bash
  code .
  ```

</br>

## Known Bugs

* No known bugs

<br>

## License

MIT License

Copyright (c) 2022 Ruben Giosa, Reed Carter, Chloe (Yen Chi) Le

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
