# KGR

The project is develope based on Python, and the code is implemented in Pytorch environment. The code of the project is in the src directory.

## How to Run

You can use one of the config files to train:

```shell
./experiment.sh configs/${config_file}.sh --train gpu_id
```

And you can use the following commad to evaluate:

```shell
./experiment.sh configs/${config_file}.sh --inference gpu_id
```

## Data Format



The data is originated from [Matweb](http://www.matweb.com/search/MaterialGroupSearch.aspx) and you can get the dataset in the data directory.  The KG triples are represented in the format `head_entity tail_entity relationship`. If you want to make your own dataset, the data format is required. And all the inverse triples corresponding to the fact should be added in the KG.

