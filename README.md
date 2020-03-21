# W251 Final Project - Fall Detection (Inference using TSM)



## SETUP

Build docker image
```
docker build -t tsm_hand -f Dockerfile.tsm .
```

Create container
```
docker run --name tsm --privileged -v "$PWD"/temporal-shift-module:/temporal-shift-module -ti tsm_hand bash
```

Run main.py in temporal-shift-module
```
cd temporal-shift-module
python3 main.py
```
