# volunteer_match

## Generated data
This folder contains data generated by the [volunteer_match project](https://github.com/fjhheras/volunteer_match).

## Directory structure
    .
    ├── readme.md
    ├── ratings_train.csv                       # Generated by `generate_ratings_train.py`
    ├── tasks_vectors.pkl                       # Generated by `script_precompute_vectors.py`
    ├── tasksnointro_vectors.pkl                # Generated by `script_precompute_vectors.py`
    ├── volunteers_vectors.pkl                  # Generated by `script_precompute_vectors.py`
    ├── tasks_deep_embedding.pkl                # Generated by `script_neural_network_embedding.py`
    ├── volunteers_deep_embedding.pkl           # Generated by `script_neural_network_embedding.py`
    ├── tasks_with_cluster_affinities.csv       # Generated by `script_neural_network_cluster.py`
    ├── volunteers_with_cluster_affinities.csv  # Generated by `script_neural_network_cluster.py`
    ├── cluster_model.pth                       # Generated by `script_neural_network_cluster.py`
    ├── requests_cluster_?.csv                  # Generated by `script_split_up_clusters_to_csv.py`
    ├── volunteers_cluster_?.csv                # Generated by `script_split_up_clusters_to_csv.py`
    └── tasks_form_cluster_?.csv                # Generated by `script_split_up_clusters_to_csv.py`

