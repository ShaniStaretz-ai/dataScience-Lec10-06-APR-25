# dataScience-Lec10-06-APR-25
End of pandas, start of graphs
* Time functions: presentation 22
  * to_datetime: convert string to dateTime 
    * if it's not in the right format,to convert seiers of string to dateTime object, need to convert to the right format with optional parameter:
      * pd.to_datetime(s,format='%d--%m--%y')
      ![img_4.png](img_4.png)
      * b= month in word
      * M= month
      * m=minutes
      * H= 24 format
      * h=12 format
  * then you can do the actions on the datetime objects:
    * resample(rule=<A>) group by rule value
      * rule: 
      * rule values:
      * A=annual
      ![img.png](img.png)
      *  
  * back to string: 
    * ![img_1.png](img_1.png)
  * all other actions from datetime class, like in python:
    * ![img_2.png](img_2.png) - if the date is not index
    * ![img_3.png](img_3.png) if date is index
  * in case of different format: 
    * the function to_datetime need to identify the input's format, 
    * in order to convert to datetime object, therefore need to provide the list of possible formats. 
    if it doesn't recognize will try the next format or set value of NaT/NaN
* pivot table:  presentation 23
  * another way to groupby and run aggregation action on the data  per index and display
  * it's like groupby by 2 groups: the first is index, and the second the columns.
  ![img_5.png](img_5.png)
  * since the first action is lambda, the result will be like:
  ![img_6.png](img_6.png)
    * therefore use for loop : ![img_8.png](img_8.png) 
    and then rename the column:    ![img_10.png](img_10.png)
  * save the df to external file df.to_csv/html/excel (file):
  * ![img_9.png](img_9.png)
## Matplotlib Library: visualization library
![img_7.png](img_7.png)

    