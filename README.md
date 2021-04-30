# HF_metrics

[script.py](script.py) takes as an input the data files (in .csv format) related to the HF protocols for both with and without the use of exoskeleton. Datafile names should be provided with .csv extension and relative to where the script is run from. Arguments related to the execution time for asending/descending task are also required as an input.

It then computes the related metrics. It also optionally accepts the output filename (in .yaml format). 

## USE
The command for using the script is below:
```
python script.py --exo_datafile FILENAME_EXO --noexo_datafile FILENAME_WITHOUT_EXO 
--exo_task_time TASK_TIME_EXO --noexo_task_time TASK_TIME_WITHOUT_EXO
--output_file FILENAME_OUT
```

If using the datafile named subject-1.csv, the command to run the script should be:

```
python script.py --exo_datafile subject-1.csv --noexo_datafile subject-1.csv 
--exo_task_time 120 --noexo_task_time 150 --output_file HR_metrics.yaml
```
