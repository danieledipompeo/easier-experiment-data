
## Run a Docker image

 - Experiment: 
   - Case study: train-ticket
   - Algorithm: nsgaii
   - Search Budget: none
   - Search Budget Threshold: 6000

 - Analysis outcome

```
Centroid: 289
perfQ          0.326796
reliability    0.781316
#changes           5.99
pas                 2.0

					  label  solID
289            fast / reliable / very-few / few   1813

Name: 289, dtype: object
nsgaii-train-ticket-sbspe-100-eval-it-0/objectives/FUN19__train-ticket__BRF_clone_1.23__moc_1.64__mcnn_1.80__moncnn_1.45__MaxEval_100__ProbPAs_0.95__sb_none_sbth_6000__Algo_nsgaii.csv
```

docker pull danieledipompeo/easier:sbspe; for i in $(seq 1 31); do docker run -d --log-driver=journald --rm --mount type=tmpfs,destination=/tmp -v /mnt/data/easier/nsgaii-train-ticket-sbspe-100-eval-it-1-centroid-289/run$i:/mnt/easier-output/ danieledipompeo/easier:sbspe https://raw.githubusercontent.com/danieledipompeo/easier-experiment-data/main/nsgaii-train-ticket-sbspe-100-eval-it-1-centroid-289/config.ini iteration-mode; done

