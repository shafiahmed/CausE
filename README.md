# CausE

Python code for the RecSys 2018 paper entitled 'Causal Embeddings for Recommendation' using Tensorflow. A pre-print version of the paper can be found here - https://arxiv.org/abs/1706.07639


## Code Organisation
The code is organized as follows:
- **models.py** - SupervisedProd2Vec and CausalProd2Vec as tensorflow model classes.
- **dataset_loading.py** - File to load Movelens/Netflix datasets and convert to user/product matrix.

## Dependencies and Requirements
The code has been designed to support python 3.6+ only. The project has the following dependences and version requirements:

- python3 - 3.6.5+
- tensorflow - 1.9.0+
- tensorboard - 1.9.0+
- numpy - 1.14.5+
- scipy - 1.1+
- pandas - 0.22+

## Datasets and Pre-processing

We make use of the MovieLens100K and 10M datasets to present results for our paper. Both datasets can be downloaded from here - https://grouplens.org/datasets/movielens/

Both MovieLens datasets can then be converted into a format compatible for our approach using the gen_dataset.py script. 

## Training a Model



### Optional arguments

The code uses TF flags to manage the command line arguments for running the models, please note that both models have the same parameters.

> Causal Embeddings for Recommendation Parameters 
>
>optional arguments: <br />
> --data_set : The dataset to load <br />
>  --model_name The name of the model used when saving (default: cp2v) <br />

## License

Copyright CRITEO

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and limitations under the License.
