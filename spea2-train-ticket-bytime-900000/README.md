
## Run a Docker image

 - Experiment: 
   - Case study: train-ticket
   - Algorithm: spea2
   - Search Budget: byTime
   - Search Budget Threshold: 900000

docker pull danieledipompeo/easier:v1.0; for i in $(seq 1 31); do docker run -d --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/spea2-train-ticket-bytime-900000/run$i:/mnt/easier-output/ danieledipompeo/easier:v1.0 https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/spea2-train-ticket-bytime-900000/config.ini; done

