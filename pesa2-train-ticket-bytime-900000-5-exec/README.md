
## Run a Docker image

 - Experiment: 
   - Case study: train-ticket
   - Algorithm: pesa2
   - Search Budget: byTime
   - Search Budget Threshold: 900000

docker pull danieledipompeo/easier:v1.0; for i in $(seq 1 1); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/pesa2-train-ticket-bytime-900000-5-exec/run$i:/mnt/easier-output/ danieledipompeo/easier:v1.0 https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/pesa2-train-ticket-bytime-900000-5-exec/config.ini; done

