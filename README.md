# manta_dev
This repository is meant to collect and keep track of the different repositories that exist for Manta.

## Downloading

1. Clone the repository
	```bash
	$ git clone git@github.com:vortexntnu/manta_dev.git
	```

2. Initialize the submodules
    ```bash
	$ cd ~/manta_ws/src/manta_dev/
	```
	```bash
	$ git submodule update --init --recursive
	```

After cloning this repository, navigate into manta_dev and run the command "git submodule update --init"

## Important when building

If you do not have cuda remember to add touch CATKIN\_IGNORE in darknet\_ros.
1. Navigate to home
	```bash
	$ cd
	```

2. Add CATKIN_IGNORE
	```bash
	$ touch manta_ws/src/manta_dev/darknet_ros/CATKIN_IGNORE
	```

## How to use

When the master branch of the subrepo is updated it is necessary to update which commit this repository points to. Be careful not to update this repo to point to a specific branch instead of the master branch.
1. Navigate to manta_dev
	```bash
	$ cd ~/manta_auv/src/manta_dev/
	```

2. Stage for commit
	```bash
	$ git add "subrepo"
	```

3. Commit
	```bash
	$ git commit -m 'Commit message here'
	```

4. Push to master
	```bash
	$ git push origin master
	```
