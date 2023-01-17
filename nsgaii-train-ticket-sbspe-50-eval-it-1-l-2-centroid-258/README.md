
## Run a Docker image

 - Experiment: 
   - Case study: train-ticket
   - Algorithm: nsgaii
   - Search Budget: none
   - Search Budget Threshold: 6000

 - Analysis outcome

```
Centroid: 258
perfQ          0.208608
reliability    0.302645
#changes           3.28
pas                 0.0

                                               label  solID
258  fast / minimally-reliable / very-few / very-few   1334

Name: 258, dtype: object
/content/datasets/nsgaii-train-ticket-sbspe-50-eval-it-0-l-2/objectives/FUN17__train-ticket__BRF_clone_1.23__moc_1.64__mcnn_1.80__moncnn_1.45__MaxEval_50__ProbPAs_0.95__sb_none_sbth_6000__Algo_nsgaii.csv
```

docker pull danieledipompeo/easier:sbspe; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii-train-ticket-sbspe-50-eval-it-1-l-2-centroid-258/run$i:/mnt/easier-output/ danieledipompeo/easier:sbspe https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii-train-ticket-sbspe-50-eval-it-1-l-2-centroid-258/config.ini iteration-mode; done

