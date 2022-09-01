# Sientia-BI
Business Iintelligent solution that leverage data driven insights and decision making in OT environments 

# How to install and run

  1. Install Docker desktop version [link](https://www.docker.com/products/docker-desktop/)
  
  2. Run docker desktop
  
  3. Unzip the *Metabase-Airflow.zip* file in the root folder of the repo (the unzipped documents have the docker files and also the iris data set that will be used as an example)
  
  4. Open your terminal command in the folder where you unzipped the files from *Metabase-Airflow.zip*
  
  5. Run the following command
  
  ```
  docker compose up
  ```
  
  6. Wait for the long installation process
  
  7. Open [Minio](https://min.io/) via localhost at:
  
  ```
  http://localhost:9001/
  
  user: minioadmin
  pass: minioadmin
  ```

  8. In the Bucket tab, ceate buckets **curated** and **landing** ![Minio bucket creation](/figures/MicrosoftTeams-image%20(1).png)
  
  9. Upload the data files from this repo (*iris-1.csv* and *iris-2.csv*) to the **landing** bucket that you have just created 
  
  10. Now open [Airflow](https://airflow.apache.org/) web page at:
  
  ```
  http://localhost:8080/
  
  user: airflow
  pass: airlfow
  ```
  
  11. Run the airflow as the figure below is showing: ![airflow_picture](/figures/MicrosoftTeams-image%20(2).png)
  
  # Accessing and configuring the applications
  
  1. Configure Metabase connection to the Postgree database as shown 
  


