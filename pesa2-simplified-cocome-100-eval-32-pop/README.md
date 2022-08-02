
## Run a Docker image

 - Experiment: 
   - Case study: simplified-cocome
   - Algorithm: pesa2
   - Search Budget: none
   - Search Budget Threshold: 900000

docker pull danieledipompeo/easier:v1.1; for i in $(seq 1 30); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/pesa2-simplified-cocome-100-eval-32-pop/run$i:/mnt/easier-output/ danieledipompeo/easier:v1.1 https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/pesa2-simplified-cocome-100-eval-32-pop/config.ini; done

