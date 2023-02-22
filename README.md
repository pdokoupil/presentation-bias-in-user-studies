# Rows or Columns? Minimizing presentation bias while comparing multiple recommenders.
This repository contains raw results and supplementary materials for the paper "Rows or Columns? Minimizing presentation bias while comparing multiple recommenders" submitted to SIGIR 2023. The main aim of the paper is to characterize how presentation bias affects different layouts of page-based within-subject user studies on recommender systems. 

### This repository contains:
- raw results of the user study (processed into Python's pickle files with some sensitive attributes removed)
  - note that due to the filesize limitations, the file interaction_data.zip needs to be unziped first
- notebooks for replication of the presented results on both low-level and high-level feedback. Notebooks also contain several additional analysis that were removed for the sake of space (see also the "plots" folder for generated visualizations).
- samples from the user study website (see "study_website_samples" folder). Note that the study website cannot be published due to the anonymization, but it will be included after the review period)
- [requirements.txt](./requirements.txt) file
  - note that we ran the experiments with Python 3.9.6 but any reasonably new version of Python3 should work fine

### Reproducing the results
All input data (interactions, participant data) and notebooks for generating all the results (and plots) mentioned in the paper are present in this repository, therefore if we take the input data as given then the results are easily reproducible.

By the very nature of user studies, the obtained input data would differ for different sets of participants and therefore cannot be reproduced exactly. Nonetheless, the [source codes](https://anonymous.4open.science/r/grs-user-studies-774E/README.md) necessary to run the user study are available, so at the same study setting is easy to reproduce.
  - Running the website can be done easily by first building the docker container (using `build_server_container.sh`) and then running the container (using `start_server.sh`). Participants view of the study is then accessible from the following link (replace `127.0.0.1` with appropriate hostname): `http://127.0.0.1:5000/plugin1/join?guid=18AiOQ-PGIXZm5oX6qIWzQq3NcK6g0po`

