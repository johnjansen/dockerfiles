# wp-download wrapped in a container

    docker run -it --rm --volume="/Users/johnjansen/Downloads/wp-d-dump:/wikipedia" johnjansen/wikipedia_extractor --custom-dump en:20160305

see https://github.com/babilen/wp-download for more details