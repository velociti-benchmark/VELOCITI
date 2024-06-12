<img src="assets/run.ico" width=70 height=70/> 

# VELOCITI: Can Video Language Models Bind Semantic Concepts Through Time?


## Welcome to the VELOCITI, this repository is to provide code for Evaluation of models on VELOCITI, and provide a jupyter notebook to visualize all the data presented in the benchmark.

### ⭐️ For instant visualization of data samples, please visit our project page: [velociti-benchmark.github.io](velociti-benchmark.github.io)


# Set-Up for Visualizing Data

### Setting-up the Conda Environment
```
conda env create --name veloexplore --file environments/visualizer_env.yaml
conda activate veloexplore
```

### Setting-up Data

- The data is available [Here](https://drive.google.com/file/d/1kwXbOknTZA-BeUbpXH5tSS77kiBTipkt/view?usp=drive_link) as a `.zip` file.
- Either manually visit the link and donwload the `velociti_data.zip` in the root of this directory, or
- Download the `velociti_data.zip` via `gdown`

```
pip install gdown
cd VELOCITI
```
Then in a python terminal or a file,

```
import gdown
gdown.download('https://drive.google.com/uc?id=1kwXbOknTZA-BeUbpXH5tSS77kiBTipkt', 'velociti_data.zip')
```

Unzip the data, and you should see the directory structure as below.

#### Unzip the contents of the `.zip`, and ensure the following directory structure

```
.
├── LICENSE.txt
├── data
│   ├── action_adv.json
│   ├── action_bind.json
│   ├── action_mod.json
│   ├── agent_bind.json
│   ├── agent_iden.json
│   ├── control.json
│   ├── coref.json
│   ├── pos_caps.json
│   ├── sequence.json
│   └── vidsitu_dict.json
├── data_explore.ipynb
├── velociti_data.zip
└── videos
    ├── velociti_videos_10s
    └── velociti_videos_4s
```


Ready for browsing the [provided Jupyter Notebook](data_explore.ipynb) !


<hr>

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
