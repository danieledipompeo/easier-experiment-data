
## Run a Docker image

 - Experiment: 
   - Case study: 
   - Algorithm: nsgaii
   - Search Budget: none
   - Search Budget Threshold: 6000

 - Analysis outcome

```
Centroid: 317
perfQ          0.216461
reliability    0.759612
#changes           3.28
pas                10.0

                                         label  solID
317      fast / very-reliable / very-few / few   1419

Name: 317, dtype: object
/content/datasets/nsgaii-cocome-sbspe-50-eval-it-0-l-2/objectives/FUN20__simplified-cocome__BRF_clone_1.23__moc_1.64__mcnn_1.80__moncnn_1.45__MaxEval_50__ProbPAs_0.95__sb_none_sbth_6000__Algo_nsgaii.csv
```

docker pull danieledipompeo/easier:sbspe; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii-cocome-sbspe-50-eval-it-1-l-2-centroid-317/run$i:/mnt/easier-output/ danieledipompeo/easier:sbspe https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii-cocome-sbspe-50-eval-it-1-l-2-centroid-317/config.ini iteration-mode; done

