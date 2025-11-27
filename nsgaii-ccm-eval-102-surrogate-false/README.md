
## Run a Docker image

 - Experiment: 
   - Case study: 
   - Algorithm: pesa2
   - Search Budget: none
   - Search Budget Threshold: 900000

docker pull danieledipompeo/easier:surrogate; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii-ccm-eval-102-surrogate-false/run$i:/mnt/easier-output/ danieledipompeo/easier:surrogate https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii-ccm-eval-102-surrogate-false/config.ini modelling-energy; done 

