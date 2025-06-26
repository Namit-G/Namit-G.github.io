+++
date = '2025-06-26T19:56:16+05:30'
draft = false
title = 'Index'
+++

---

![Pipeline Screenshot](/images/spacex-dag.png)

### What was the challenge?  
The SpaceX launch data was available via REST APIs but lacked context, structure, and reliability. Manual scraping wasn’t scalable.

### What I built  
I architected an automated ETL pipeline using Python and Apache Airflow. The pipeline fetched SpaceX data daily, normalized schema, and generated mission insights via dashboards.

### Key technical decisions  
- Used Airflow’s `HttpSensor` to check for data freshness  
- Added retry policies + Slack alerts for failure cases  
- Stored results in Parquet format for analytics

### Challenges I overcame  
- API rate-limits → added caching layer  
- Data schema drift → implemented dynamic schema handling  
- Debugging DAG failures in cloud deployments

### Tech used  
Python • Apache Airflow • REST APIs • Docker • Parquet

🔗 [GitHub Repository](https://github.com/Namit-G/SpaceX-Data-Pipeline)
