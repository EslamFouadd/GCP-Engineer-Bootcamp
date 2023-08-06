### What Are Our Data Quality Issues?

1. **Data Quality Issue #1**:  
> **Missing Values**:
Each feature column has multiple missing values.  In fact, we have a total of 18 missing values.

2. **Data Quality Issue #2**: 
> **Date DataType**:  Date is shown as an "object" datatype and should be a datetime.  In addition, Date is in one column.  Our business requirement is to see the Date parsed out to year, month, and day.

3. **Data Quality Issue #3**: 
> **Model Year**: We are only interested in years greater than 2006, not "<2006".

4. **Data Quality Issue #4**:  
> **Categorical Columns**:  The feature column "Light_Duty" is categorical and has a "Yes/No" choice.  We cannot feed values like this into a machine learning model.  In addition, we need to "one-hot encode the remaining "string"/"object" columns.

5. **Data Quality Issue #5**:  
> **Temporal Features**:  How do we handle year, month, and day?
