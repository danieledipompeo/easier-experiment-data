
## Run a Docker image

 - Experiment: 
   - Case study: simplified-cocome
   - Algorithm: nsgaii
   - Search Budget: none
   - Search Budget Threshold: 900000

docker pull danieledipompeo/easier:v1.1; for i in $(seq 1 30); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii-simplified-cocome-10-eval/run$i:/mnt/easier-output/ danieledipompeo/easier:v1.1 https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii-simplified-cocome-10-eval/config.ini; done

