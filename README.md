# AI-Dissertation
My Computer Science Dissertation
The project will already have neural networks attached so you can just go ahead and press play, but if you wish to see what 
training looks like, or create new trained neural network files go through these steps/commands in a command line then press play.
Please let me know if you have issues importing/running the project that aren't performance based!

Firstly change directory to project directory (this example uses my project directory, so keep yours in mind for the steps):
cd D:\Documents\My project (1)\

start virtual python environment:
python-envs\sample-env\Scripts\activate

start mlagents, --force is used to overwrite previously generated artifact without having to specify a new artifact name:
mlagents-learn --force

under current settings generated tracker neural network will be under:
\My project (1)\Assets\results\ppo\trackerconfig

and generated avoider neural network will be under:
D:\Documents\My project (1)\Assets\results\ppo\


to run a specific config file you put the url to the yaml config file and the run id, or --force for the same reason as
earlier: 
mlagents-learn config/ppo/rollerball_config.yaml --force
mlagents-learn config/ppo/rollerball_config.yaml --run-id=RollerBall

Unity mlagents reference:
@article{juliani2020,
  title={Unity: A general platform for intelligent agents},
  author={Juliani, Arthur and Berges, Vincent-Pierre and Teng, Ervin and Cohen, Andrew and Harper, Jonathan and Elion, Chris and Goy, Chris and Gao, Yuan and Henry, Hunter and Mattar, Marwan and Lange, Danny},
  journal={arXiv preprint arXiv:1809.02627},
  url={https://arxiv.org/pdf/1809.02627.pdf},
  year={2020}
}