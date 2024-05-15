
## Run a Docker image

 - Experiment: 
   - Case study: 
   - Algorithm: pesa2
   - Search Budget: none
   - Search Budget Threshold: 6000

docker pull danieledipompeo/easier:energy; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/pesa2-ttbs-aws-energy-eval-200-baseline/run$i:/mnt/easier-output/ danieledipompeo/easier:energy https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/pesa2-ttbs-aws-energy-eval-200-baseline/config.ini modelling-energy; done 

