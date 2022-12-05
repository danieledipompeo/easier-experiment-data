
## Run a Docker image

 - Experiment: 
   - Case study: 
   - Algorithm: nsgaii
   - Search Budget: none
   - Search Budget Threshold: 6000

docker pull danieledipompeo/easier:sbspe; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii-cocome-sbspe-1000-eval/run$i:/mnt/easier-output/ danieledipompeo/easier:sbspe https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii-cocome-sbspe-1000-eval/config.ini support-workload; done

