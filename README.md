# W251 Final Project - Fall Detection (Inference using TSM)



## SETUP

Clone the original TSM repo here
```
git clone https://github.com/mit-han-lab/temporal-shift-module.git
```

Build docker image
```
docker build -t tsm_hand -f Dockerfile.tsm .
```

Create container
```
docker run --name tsm --privileged -v "$PWD":/tsm_vol -v "$PWD"/temporal-shift-module:/temporal-shift-module -ti tsm_hand bash
```

Run main.py in temporal-shift-module
```
cd temporal-shift-module
python3 main.py
```
