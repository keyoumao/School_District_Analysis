# School_District_Analysis
## PySchool
## Challenge

### We have updated the student_data_df with NaN for all for ninth graders at Thomas High School, and then merged clean student data with the school dataset. The remaining tasks can be completed in a similar to the Module.

#### After replacing the reading and math scores, complete the following steps and answer the questions for each step. 
##### Recreate the district and school summary DataFrames

1. How is the district summary affected?
---------------------------------------------------------------------------------------------------------
        Average Math Score	Average Reading Score	% Passing Math	% Passing Reading	% Overall Passing (overall)
        79.0	              81.9	                75	            86	              65         Before
        78.9	              81.9	                74	            85	              64         After       
---------------------------------------------------------------------------------------------------------
   From the above table, we could see that the average Math Score has dropped by 0.1; Average Reading Score maintained the same; Passing percentage for both Math and Reading dropped by 1%; Overall Passing percentage has dropped by 1%. 

2. How is the school summary affected?
---------------------------------------------------------------------------------------------------------
        Average Math Score	Average Reading Score	% Passing Math	% Passing Reading	% Overall Passing (Thomas)
        83.4	              83.8	                93	            97	              91         Before
        83.4	              83.9	                67	            70	              65         After       
---------------------------------------------------------------------------------------------------------
   The updated dataframe only affects Thomas High School. The average scores do not vary but all of the passing percentage have dropped drastically. 

##### Recalculate the high- and low-performing schools.
3. How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools
  See No. 2. The replacement of data does not affect other schools. Before data replacement, Thomas High School was ranked on No.2. After data replacement, Thomas High School is neither the top five or the bottom five schools based on the ranking of overall passing percentage.

##### Recalculate the scores by grade, scores by school spending, scores by school size, and scores by school type.
4. How does replacing the ninth-grade scores affect the following?
- Math and Reading Scores by Grade\
 Thomas High School has no score records for the 9th grade students.

- Scores by School Spending

  ---------------------------------------------------------------------------------------------------------
        Average Math Score	Average Reading Score	% Passing Math	% Passing Reading	% Overall Passing 
        (Before)
        <$584	    83.5	    83.9	                93	            97	              90
        $585-629	81.9	    83.2	                87	            93	              81
        $630-644	78.5	    81.6	                73	            84	              63*
        $645-675	77.0	    81.0	                66	            81	              54
        (After)
        <$584	    83.5	    83.9	                93	            97	              90
        $585-629	81.9	    83.2	                87	            93	              81
        $630-644	78.5	    81.6	                67	            77	              56*
        $645-675	77.0	    81.0	                66	            81	              54       
  ---------------------------------------------------------------------------------------------------------
  It should be notified that Thomas High School is in the range of $630-644 (marked with asterisk): average scores do not change, but the passing percentage for math, reading and overall dropped. 

- Scores by School Size
  
    ---------------------------------------------------------------------------------------------------------
        Average Math Score	Average Reading Score	% Passing Math	% Passing Reading	% Overall Passing 
        (Before)
        Small 
        (<1000)	 83.8	      83.9	                94	            96	              90
        Medium 
        (1000-2000)	83.4	  83.9	                94	            97	              91*
        Large 
        (2000-5000)	77.7	  81.3	                70	            83	              58
        (After)
        Small 
        (<1000)	 83.8	      83.9	                94	            96	              90
        Medium 
        (1000-2000)	83.4	  83.9	                88	            91	              85*
        Large 
        (2000-5000)	77.7	  81.3	                70	            83	              58    
  ---------------------------------------------------------------------------------------------------------
    Since Thomas High School belongs to medium-size (marked with asterisk). The trend is same as previously: average scores do not change, but the passing percentage for math, reading and overall dropped. 
  
- Scores by School Type
  
  ---------------------------------------------------------------------------------------------------------
        Average Math Score	Average Reading Score	% Passing Math	% Passing Reading	% Overall Passing 
        (Before)
        Charter	  83.5	    83.9	                94	            97	              90*
        District	77.0	    81.0	                67	            81	              54
        (After)
        Charter	  83.5	    83.9	                90	            93	              87*
        District	77.0	    81.0	                67	            81	              54   
  ---------------------------------------------------------------------------------------------------------
     Since Thomas High School belongs to Charter type (marked with asterisk). The trend is same as previous analysis: average scores do not change, but the passing percentage for math, reading and overall dropped as a result of data replacement.
  
