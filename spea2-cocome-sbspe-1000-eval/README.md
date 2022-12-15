
## Run a Docker image

 - Experiment: 
   - Case study: 
   - Algorithm: spea2
   - Search Budget: none
   - Search Budget Threshold: 6000

docker pull danieledipompeo/easier:sbspe; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/spea2-cocome-sbspe-1000-eval/run$i:/mnt/easier-output/ danieledipompeo/easier:sbspe https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/spea2-cocome-sbspe-1000-eval/config.ini support-branch; done

