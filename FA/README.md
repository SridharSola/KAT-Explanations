# Knowledge based Ad hoc Teamwork

This code is modfied and used for this project from the original [KAT repo](https://github.com/hharithaki/KAT/tree/main).

## Folder structure

```bash
.
├── ASP                     # ASP source files for the ad hoc agent--------------------most modifications are made here
├── gym_fortattack          # Fort Attack domain implementation files
├── malib                   # Configuration files
├── models                  # Models of other agents
├── multiagent              # Fort Attack domain implementation files--------------------some modifications made here
├── action_policy.py        # Set action policies for other agents
├── ad_hoc.py               # Ad hoc agent implementation-------------------------------modified for explanation specific output
├── arguments.py            # Default argument setup
├── fortattack.py           # Main source file
├── policies.py             # Policies for other agents
├── README.md
├── requirements.txt        # Required packages
└── utils.py                # Utility file
```

## Installation
Create an anaconda environment with python 3.6 using the following command:

```setup
conda create -n fortattack python=3.6 pip
```

Activate the enviorenment and install the required packages by executing following:

```setup
conda activate fortattack
pip install -r requirements.txt
```

Please also install opencv-contrib-python separately from source for better results. Also install an arpack in the fortattack environment and clingo in the base environment.
## Running the Code
Use the following command to run the simulation environment with ad-hoc agent, two guards, three attackers.

```setup
python fortattack.py --test
```

