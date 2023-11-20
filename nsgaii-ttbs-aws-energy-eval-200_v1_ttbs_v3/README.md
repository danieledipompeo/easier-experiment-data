
## Run a Docker image

 - Experiment: 
   - Case study: 
   - Algorithm: nsgaii
   - Search Budget: none
   - Search Budget Threshold: 6000

docker pull danieledipompeo/easier:energy; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii-ttbs-aws-energy-eval-200_v1_ttbs_v3/run$i:/mnt/easier-output/ danieledipompeo/easier:energy https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii-ttbs-aws-energy-eval-200_v1_ttbs_v3/config.ini modelling-energy; done 

