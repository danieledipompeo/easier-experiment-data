
## Run a Docker image

 - Experiment: 
   - Case study: simplified-cocome
   - Algorithm: nsgaii
   - Search Budget: none
   - Search Budget Threshold: 6000

docker pull danieledipompeo/easier:sbspe; for i in $(seq 1 30); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii__cocome__10_eval__16_popsize__sbspe__20_260/run$i:/mnt/easier-output/ danieledipompeo/easier:sbspe https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii__cocome__10_eval__16_popsize__sbspe__20_260/config.ini CASE_STUDY_BRANCH; done

