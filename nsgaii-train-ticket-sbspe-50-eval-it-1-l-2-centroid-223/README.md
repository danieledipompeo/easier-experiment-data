
## Run a Docker image

 - Experiment: 
   - Case study: train-ticket
   - Algorithm: nsgaii
   - Search Budget: none
   - Search Budget Threshold: 6000

 - Analysis outcome

```
Centroid: 223
perfQ          0.205996
reliability    0.788695
#changes            2.9
pas                 2.0

                                               label  solID  
223        fast / very-reliable / very-few / average    584  

/content/datasets/nsgaii-train-ticket-sbspe-50-eval-it-0-l-2/objectives/FUN14__train-ticket__BRF_clone_1.23__moc_1.64__mcnn_1.80__moncnn_1.45__MaxEval_50__ProbPAs_0.95__sb_none_sbth_6000__Algo_nsgaii.csv
```

docker pull danieledipompeo/easier:sbspe; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii-train-ticket-sbspe-50-eval-it-1-l-2-centroid-223/run$i:/mnt/easier-output/ danieledipompeo/easier:sbspe https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii-train-ticket-sbspe-50-eval-it-1-l-2-centroid-223/config.ini iteration-mode; done

