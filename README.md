# ETH Quantum Hackathon 2024 - QuEra & MOODY'S Challenge

Here you will learn all the details needed to operate QuEra resources for ETH Quantum Hackathon 2024. See [`challenge.md`](challenge.md) to find out about the actual challenge.


The folder [tutorial/](tutorial/) contains material related to the presentation of the ETH Quantum Hackathon workshop on Saturday morning.

Check also the [references/](references/) folder for papers that may be relevant for you. If useful, the authors of the original work in which this challenge is based have also documented their code quite clearly in [this  GitHub repo](https://github.com/jpmorganchase/hardness-of-mis-on-udg). But beware: time for this challenge is short, so make sure to not get lost in navigating too much content!

## Installing Bloqade and other packages 

Bloqade, QuEra's neutral atom emulator and SDK, is going to be the key software you will operate for this challenge. Bloqade has both Julia-based and Python-based versions and we suggest focusing on the latter here.Installing Bloqade-python involves a simple `pip install bloqade`.

Guidelines for the Julia version can also be found [here](https://queracomputing.github.io/Bloqade.jl/dev/), and this can be relevant for advanced classical simulation and theoretical analysis. Another of QuEra's packages for graph problems that may be useful to you is Generic Tensor Networks; instructions can be found [here](https://queracomputing.github.io/GenericTensorNetworks.jl/dev/). It is also based on Julia language.

## Debugging and technical support

To make sure you have access to debugging and technical support from QuEra's team, make sure at least 1 person of your team connects to [QuEra's public Slack workspace](https://querapublic.slack.com/join/shared_invite/zt-1r86wjwxs-OcdmXqBOisO~AHISXTL80w#/shared-invite/email). There you should be able to reach to John Long or Pedro Lopes for technical help.

Be sure to DM Pedro or John to be included in the `eth-zurich-hackathon` channel for broad event announcements.

Notice that your account IDs will be distributed via DM on the QuEra's public Slack workspace! If you want to use Aquila, registering at least 1 team member is mandatory.

## Accessing Aquila
In this event, you will have access to Aquila, QuEra's analog neutral-atom quantum computer! For that, we suggest using either python scripts or notebooks. Yet, to ensure your jobs do not get stuck in the long queue that seems to be coincident with the event, you will need to activate what are known as `hybrid` workflows on Amazon Braket. The original goal of hybrid workflows is to enable more performant variational algorithms. For us, it will just serve as a means to cut the line and get your results quicker.

To help you understand how to submit `hybrid` jobs to Aquila, we prepared the following [tutorial guidelines](assets/bloqade-braket-submission-guide.ipynb).

## Quantum resources availability and code of conduct
To guarantee fair sharing of resources among teams, here are the guidelines for usage of QuEra's quantum computing resources during the hackaton:
* *Each group has a total of $100 USD in credits. The cost of a given job is given by $0.3 x number of tasks + $0.01 x number of shots/task x number of tasks. Calculate your own expenses!* 
* Tasks are to be limited to **100 repetition shots**.
* Hybrid optimization jobs will **not** be allowed.
* Aquila will be continuously available to participants.


## Documentation

This year’s ETH Quantum Hackathon challenges require a write-up/documentation portion that is heavily considered during judging. The write-up is a chance for you to be creative in describing your approach and describing your process. It should clearly explain the problem, the approach you used, your implementation with results from simulation and hardware, and how you accessed the quantum hardware (total number of shots used, backends used, etc.).

Make sure to clearly link the documentation into the `README.md` of your own solutions folder and to include a link to the original challenge repository from the documentation!


## Submission

To submit the challenge, do the following:
1. Place all the code you wrote in one folder with your team name under the `team_solutions/` folder (for example `team_solutions/quantum_team`).
2. Create a new entry in `team_solutions.md` following the format shown that links to the folder with your solution and your documentation.
3. Create a Pull Request from your repository to the original challenge repository
4. Submit the "challenge submission" form

Project submission forms will automatically close on Sunday at 11:30AM CET and won't accept late submissions.
