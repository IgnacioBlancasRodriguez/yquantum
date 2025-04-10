# Read Me

Here you will learn all the details needed to operate QuEra resources for YQuantum 2024. See [`challenge.md`](challenge.md) to find out about the actual challenge.


The folder [tutorial/](tutorial/) contains material related to the presentation of the workshop.

Check also the [references/](references/) folder for papers that may be relevant for you. But beware: time for this challenge is short, so make sure to not get lost in navigating too much content!

## Installing Bloqade and other packages 

Bloqade, QuEra's neutral atom emulator and SDK, is going to be the key software you will operate for this challenge. Bloqade has both Julia-based and Python-based versions and we suggest focusing on the latter here.

For this event, you will need to operate it from inside qBraid's platform, but if you want to run emulations by yourself, you can easily install Bloqade locally via `pip install bloqade`.

Guidelines for the Julia version can also be found [here](https://queracomputing.github.io/Bloqade.jl/dev/). Another of QuEra's packages for graph problems that may be useful to you is Generic Tensor Networks; instructions can be found [here](https://queracomputing.github.io/GenericTensorNetworks.jl/dev/). It is also based on Julia language.

## Working on qBraid

While simulations and emulations of your program can be done locally on your computer, operation of QuEra's systems for this event will mandatorily go via qBraid (where you can also do the emulations, if you want). So here are some guidelines:

1. To launch these materials on qBraid, first fork this repository and click the above `Launch on qBraid` button. It will take you to your qBraid Lab with the repository cloned.
2. Once cloned, open terminal (first icon in the **Other** column in Launcher) and `cd` into this repo. Set the repo's remote origin using the git clone url you copied in Step 1, and then create a new branch for your team:
```bash
cd  2024_QuEra
git remote set-url origin <url>
git branch <team_name>
git checkout <team_name>
```

3. Use the environment manager (**ENVS** tab in the right sidebar) to [install environment](https://qbraid-qbraid.readthedocs-hosted.com/en/latest/lab/environments.html#install-environment) "Amazon Braket". The installation should take ~2 min.
4. Once the installation is complete, click **Activate** to [add a new ipykernel](https://qbraid-qbraid.readthedocs-hosted.com/en/latest/lab/kernels.html#add-remove-kernels) for "Amazon Braket".
5. From the **FILES** tab in the left sidebar, double-click on the `2024_QuEra` directory.
6. You are now ready to begin hacking! Work with your team to complete either of the challenges listed above.

For other questions or additional help using qBraid, see [Lab User Guide](https://qbraid-qbraid.readthedocs-hosted.com/en/latest/lab/overview.html), or reach out on [Discord](https://discord.gg/gwBebaBZZX).

## Quantum resources availability and code of conduct
To guarantee fair sharing of resources among teams, here are the guidelines for usage of QuEra's quantum computing resources during the hackaton:
* Tasks are to be limited to **100 repetition shots**.
* Hybrid optimization jobs will **not** be allowed.
* Aquila will be continuously available to participants until *Sunday 7a.m.*


## Documentation

This year’s YQuantum challenges require a write-up/documentation portion that is heavily considered during
judging. The write-up is a chance for you to be creative in describing your approach and describing
your process. It should clearly explain the problem, the approach you used, your implementation with results
from simulation and hardware, and how you accessed the quantum hardware (total number of shots used, backends used, etc.).

Make sure to clearly link the documentation into the `README.md` of your own solutions folder and to include a link to the original challenge repository from the documentation!


## Submission

To submit the challenge, do the following:
1. Place all the code you wrote in one folder with your team name under the `team_solutions/` folder (for example `team_solutions/quantum_team`).
2. Create a new entry in `team_solutions.md` following the format shown that links to the folder with your solution and your documentation.
3. Create a Pull Request from your repository to the original challenge repository
4. Submit the "challenge submission" form

Project submission forms will automatically close on Sunday at 10am EST and won't accept late submissions.
