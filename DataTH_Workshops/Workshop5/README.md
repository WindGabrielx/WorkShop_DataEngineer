# Workshop_DataTH_Workshop5
Welcome to my workshop! In this session, I will share various case studies and practical examples from my learning journey through DataTH, an online platform offering the "Road to Data Engineer" course. The content here showcases the skills and knowledge I’ve gained. This workshop covers the following topics:

   - Differences between Table and View, and Understanding Partitioning
   - Introduction and hands-on experience with Google BigQuery
   - Loading data into BigQuery using Airflow
      - Directly imported the data file to BigQuery. (Manual method)
      - BashOperator (Automatic method)
      - GCSToBigQueryOperator (Automatic method)


     Workshop_start_ws5_bq_load:
      - BashOperator (Automatic method): I used the BashOperator to automatically import the result from our bucket to BigQuery and named the data file
        (This is in t4). 
        This process continues from "start_ws4_exercise4 (Workshop4_4)", and the task dependencies are defined as:
        [t1, t2] >> t3 >> t4, where t1 and t2 complete first, followed by t3, and then t4 runs to complete the pipeline.

     Workshop_start_ws5_gcs_to_bq:
      - GCSToBigQueryOperator (Automatic method): I used the GCSToBigQueryOperator to automatically import from our bucket to BigQuery and named the data file
        This process continues from "start_ws4_exercise4 (Workshop4_4)", and the task dependencies are defined as:
        [t1, t2] >> t3 >> t4, where t1 and t2 complete first, followed by t3, and then t4 runs to complete the pipeline.
        
         
   
