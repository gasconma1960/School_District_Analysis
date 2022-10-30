# School_District_Analysis

# Background

  Maria has gotten a new version of the student data with several changes. This includes an additional column: "school budget". She wants you to rework part of your analysis by using the new dataset.
  
 # Purpose of the Project
  Using Python, Pandas and Jupyter we are helping Maria to analyze the data for the School District, creating a clean code that runs accurate to provide that information and result to Maria
  
 # Phases of this Project  

- Deliverable 1: Collect the student data into a DataFrame.

- Deliverable 2: Prepare a cleaned version of the DataFrame.
- Deliverable 3: Summarize key pieces of the data.
- Deliverable 4: Drill down into the data to analyze specific subsets.
- Deliverable 5: Compare and contrast the data through grouping and aggregation functions.
- Deliverable 6: A written analysis of your results (README.md).

## *Deliverable 1: Collect the student data into a DataFrame* 

*1. Import the data from the new_full_student_data.csv file into a DataFrame named student_df by using the Pandas read_csv function and the os module.*

*2. Confirm that Pandas correctly imported the data by using the head function, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198851215-6abd20d7-2c5d-42a2-9baa-35e5da3e95b8.png)

### Deliverable 1 Requirements
The path to the file is built by using os.path.join
![image](https://user-images.githubusercontent.com/112348240/198851365-41e277c5-8d15-4351-8735-1d5af1251861.png)

The DataFrame is created and named student_df
![image](https://user-images.githubusercontent.com/112348240/198851403-932c2537-3da1-4d7f-97bf-bbecea919ee1.png)

The first five rows of data are displayed

![image](https://user-images.githubusercontent.com/112348240/198851415-2b94e413-7d71-4814-aa25-66b8772efc99.png)

## *Deliverable 2: Prepare the Data*
### Deliverable 2 Instructions

*1. In the student DataFrame, check for rows that have NaN (or missing) values, and remove those rows, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198851531-6eb45621-3c8f-4f31-939e-15e43dc8fd27.png)

![image](https://user-images.githubusercontent.com/112348240/198851557-f2a4f4d3-9c84-4d3a-b94e-3ab7e0a613b4.png)

*2. In the student DataFrame, check for duplicate rows, and remove them.*

![image](https://user-images.githubusercontent.com/112348240/198851599-88f9176c-b974-4272-8171-1e1f87a0331e.png)

*3. Check the data types of the columns by using the dtypes property, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198852048-0c56a38b-74c2-4d7c-a682-f2e2d93f72f8.png)

![image](https://user-images.githubusercontent.com/112348240/198852069-2ddcb911-71c0-4a23-97ed-4e8f82517f03.png)

*4. In the grade column, remove the "th" suffix from every value by using str and replace, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198852087-b08f9293-74ca-45fe-a8a3-047d0e595d7f.png)

![image](https://user-images.githubusercontent.com/112348240/198852170-3dc96ed5-9465-4539-9bfe-64c774186b8e.png)

*5.Change the "grade" column to the int type, and then verify the column types, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198852262-85b24478-ac37-4a57-9909-9b89dbbf7078.png)

![image](https://user-images.githubusercontent.com/112348240/198852536-d60a5938-d08b-496f-b17d-4367e7c186ec.png)

## *Deliverable 3: Summarize the Data*

### Deliverable 3 Instructions

*1. Generate the summary statistics for the student DataFrame by using the describe function, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198852612-e66b87ba-8baa-4648-ae0f-95299192d28a.png)

*2. Display the mean math score by using the mean function.*

![image](https://user-images.githubusercontent.com/112348240/198852697-1df86669-6257-43bb-af09-4feb96e7bd2e.png)

*3. Store the minimum reading score in min_reading_score.*

![image](https://user-images.githubusercontent.com/112348240/198852713-6edeed8f-1572-4ab0-9bae-1fe9a25f45bf.png)

*4. Display the first three rows of Columns 3, 4, and 5 by using iloc, as the following image shows:*

   A screenshot depicts the first three rows of the "school_name", "reading_score", and "math_score" columns.

![image](https://user-images.githubusercontent.com/112348240/198852780-dc116171-8417-47f0-b34a-a87f1ea586c7.png)

*5. Select the rows for Grade 9, and display their summary statistics by using loc and describe, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198853092-15d3f615-ef8b-432b-9b23-99c242f04a2f.png)

*6. Store the row with the minimum overall reading score in min_reading_row by using loc and the min_reading_score variable from Deliverable 3, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198853169-5ff081d7-7304-4be7-a3ff-48315d778386.png)

*7. Select all the reading scores from the 10th graders at Dixon High School by using loc with conditionals, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198853251-88036469-4492-47cc-a0b1-e30c140ba2b7.png)

*8. Find the mean reading score for all the students in Grades 11 and 12 combined by using conditional statements and loc or iloc.*

![image](https://user-images.githubusercontent.com/112348240/198853381-4d278131-5fb7-46b4-986d-f2c8a18afe58.png)

### Deliverable 4 Requirements
- The "grade" column is displayed.

- The first three rows of Columns 3, 4, and 5 are displayed. 

- The summary statistics for 9th graders are displayed. 

- The row that contains the minimum reading score is displayed. 

- The reading scores of the 10th graders at Dixon High School is displayed. 

- The average reading score of all the students in Grades 11 and 12 combined is calculated. 

### Deliverable 5: Compare the Data 
## Deliverable 5 Instructions

*1. Display the average budget for each school type by using the groupby and mean functions, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198853662-9eaa3faf-1ff3-4884-9b35-78eb3474def5.png)

*2. Find the total number of students at each school, and sort those numbers from largest to smallest by using the groupby, count, and sort_values functions, as the following image shows:*

![image](https://user-images.githubusercontent.com/112348240/198853690-9bf20cc2-c75f-4222-baba-8367087e9ac1.png)

*3. Find the average math score by grade for each school type by using the groupby and mean functions, as the following image shows:

![image](https://user-images.githubusercontent.com/112348240/198853771-e600b868-fa96-4b45-b233-784c036e1ed8.png)

### Deliverable 5 Requirements
- The average budget for each school type is displayed. 

- The total number of students per school is displayed in descending order. 

- The average math scores for each combination of grade and school type are displayed. 

### Deliverable 6: Report Findings 
## Deliverable 6 Instructions
  Using the provided cell, write a brief summary of your findings as follows: Write a few sentences to describe any discoveries that you made while performing your analysis. Include any additional analysis that you believe would be worthwhile.
  
  ## **Summary of the Analysis**
  After reviewing all the results, we conclude:
  
  - The Math Score average is 64.67573326141189, this include all grades and school types
  
  - The Minimun Reading Score is 10.5, this include all grades and school types
  
  - Some of the Statistics for Nine Grade are : 
    - A Total of 4132 counts in reading and math score were in this data 
    
    - The minimun score for reading is 17.900000 as well as the math score is 5.300000
    
  - The minimun score for reading was for the student showing below (all grades, school and typer were included)
  
  ![image](https://user-images.githubusercontent.com/112348240/198854188-e4884062-bd0b-4ae0-b0ac-dff784c6def4.png)
  
  - Public school has a higher Budget than Charter ones:
  
    -**Charter School Budget is 872625.656236**
  
    -**Public	School Budget is 911195.558251**
    
   - The School with the Highest Student Count is :
      - Montgomery High School with 2038 students
      
Deliverable 6 Requirements

  - In a few sentences, an understanding of the performed analysis is demonstrated.

  
