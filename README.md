# Rows or Columns? Minimizing presentation bias while comparing multiple recommenders.

### This repository contains:
- raw results of the user study (processed into .pkl with some sensitive attributes removed)
  - note that due to the filesize limitations, the file interaction_data.zip needs to be unziped first
- notebooks for processing the results analysing low-level and high-level feedback dependencies
- samples from the user study website (note that the study website cannot be published due to the anonymization, but it will be included after the review period)
- [requirements.txt](./requirements.txt) file
- note that we ran the experiments with Python 3.9.6 but any reasonably new version of Python3 should work fine

### Reproducing the results
- all input data (interactions, participant data) and notebooks for generating all the results (and plots) mentioned in the paper are present in this repository, therefore if we take the input data as given then the results are easily reproducible.
- the input data itself might be more difficult to reproduce due to the nature of user studies (even if we get exactly the same participants, they most likely behave at least a bit differently than the last time). However, we compared results on two different groups of people (people we know and participants hired from Prolific) with different demographical features and the results were comparable. So even though the exact same results may not be reproducible, the results with the same significance are reproducible. To make this reproduciblity simpler, we also make the [source code](https://anonymous.4open.science/r/grs-user-studies-774E/README.md) of the user study website that was used to gather and process all the input data available.
  - Running the website can be done easily by first building the docker container (using `build_server_container.sh`) and then running the container (using `start_server.sh`). Participants should then follow the following link (replace `127.0.0.1` with appropriate hostname): `http://127.0.0.1:5000/plugin1/join?guid=18AiOQ-PGIXZm5oX6qIWzQq3NcK6g0po`

