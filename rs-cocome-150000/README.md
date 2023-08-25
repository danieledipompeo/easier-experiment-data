
## Run a Docker image

 - Experiment: 
   - Case study: 
   - Algorithm: rs
   - Search Budget: none
   - Search Budget Threshold: 6000

docker pull danieledipompeo/easier:tactics; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/rs-cocome-150000/run$i:/mnt/easier-output/ danieledipompeo/easier:tactics https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/rs-cocome-150000/config.ini support-workload; done

