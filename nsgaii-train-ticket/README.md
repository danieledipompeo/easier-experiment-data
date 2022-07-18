
## Run a Docker image

 - Experiment: 
   - Case study: train-ticket
   - Algorithm: nsgaii
   - Search Budget: none
   - Search Budget Threshold: 6000

docker pull danieledipompeo/easier:v1.0; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii-train-ticket/run$i:/mnt/easier-output/ danieledipompeo/easier:v1.0 https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii-train-ticket/config.ini; done

