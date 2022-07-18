
## Run a Docker image

 - Experiment: 
   - Case study: simplified-cocome
   - Algorithm: rs
   - Search Budget: none
   - Search Budget Threshold: 900000

docker pull danieledipompeo/easier:v1.1; for i in $(seq 1 1); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/rs-simplified-cocome/run$i:/mnt/easier-output/ danieledipompeo/easier:v1.1 https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/rs-simplified-cocome/config.ini; done

