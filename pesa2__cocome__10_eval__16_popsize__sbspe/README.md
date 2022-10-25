
## Run a Docker image

 - Experiment: 
   - Case study: simplified-cocome
   - Algorithm: pesa2
   - Search Budget: none
   - Search Budget Threshold: 6000

docker pull danieledipompeo/easier:sbspe; for i in $(seq 1 30); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/pesa2__cocome__10_eval__16_popsize__sbspe/run$i:/mnt/easier-output/ danieledipompeo/easier:sbspe https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/pesa2__cocome__10_eval__16_popsize__sbspe/config.ini test-docker-generated; done

