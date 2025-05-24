
## Run a Docker image

 - Experiment: 
   - Case study: 
   - Algorithm: pesa2
   - Search Budget: none
   - Search Budget Threshold: 900000

docker pull danieledipompeo/easier:scenarios; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/pesa-cocome-eval-200/run$i:/mnt/easier-output/ danieledipompeo/easier:scenarios https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/pesa-cocome-eval-200/config.ini modelling-energy; done 

