# Vizier First Steps Assignment

Name:Mingli Tan                   CID:A20504621

- **Task 1**: load a dataset and take a screenshot of the result

![1695560890326](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695560890326.png)

**Task 2**: Select the detail view and look at the distributions of some columns. Then look at the column view and take a screenshot of the distribution for column `Teachers_Score`

![1695561264274](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695561264274.png)

![1695561322516](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695561322516.png)

![1695561457719](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695561457719.png)

- **Task 4**: Create a SQL cell and write a query that returns columns `Teachers_Score` and `Community_Area_Name`. SQL results can be stored as new datasets in Vizier. Call the result dataset `score_and_community`. And take a screenshot of the result.

![1695561895515](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695561895515.png)

- **Task 5**: Create a SQL cell and write a query over the over the `score_and_community` dataset that computes the result as described above. Call the result dataset `community_teacher_scores`. And take a screenshot of the result.

![1695562208039](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695562208039.png)

- **Task 6**: Create a line chart of the aggregation result by creating a plot cell and take a screenshot of the result.

![1695562613090](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695562613090.png)

- **Task 7**: Insert a new cell above the SQL cell that computes the average teacher scores (notebooks in Vizier are executed top down) by pressing the three bars below the cell number. Select *"Impute Missing Values"*, select the `score_and_community` dataset and `Teachers_Score` as the column to be imputed, and select mean as the imputation method and take a screenshot of the updated line chart.

![1695563242646](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695563242646.png)

![1695563266892](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695563266892.png)

- **Task 8** Create a Python cell at the end of the notebook and create a function called `print_avg_teachers` that uses Vizier's API to get a handle for this dataset and print all values of the `avg_teacher_score` column. *Hint: use the "Show Code Examples" buttom to see example Vizier API usage and see here for the API documention*. Then use `vizierdb.export_module` to export the function. Then create a second Python cell and use `vizierdb.get_model("print_avg_teachers")` for importing the function and then call it. Take a screenshot of the result.

![1695564501645](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695564501645.png)

![1695564542378](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695564542378.png)

- **Task 9** Create another Python cell and use Vizier's API to access the dataset `community_teacher_scores` as a DataFrame, then filter out rows where the `avg_teacher_score` is larger than or equal to `30.0` and then print the remaining rows and take a screenshot.

![1695564905944](C:\Users\谭谭\AppData\Roaming\Typora\typora-user-images\1695564905944.png)