**Managing multiple projects :**
* Create separate virtual envs for different applications running on different versions of modules, python etc.
* Use the specific virtual env for running the specific application.
(lalith)
1. Managing is done in mac and by using conda in the video. Once u install conda then check the video.

2. Conda function and environmental variable code:-

   ![1547708260154](https://github.com/adityakuppa26/Python-Notes/blob/lalith_notes/images/1547708260154.png)

3. If we remove comment line i.e.,# from last line then we can automatically activate and deactivate from multiple projects<!--check video-->.

(prvnrj)
If we are using multiple projects then it is difficult to switch in between as we need to activate and de activate for each of the project.
So there is a bash script to avoid these kind of circumstances where it automatically activates the virtual environment without the specific usage of the commands.

nano ~/.bash_profile

#!/bin/bash

# conda-auto-env automatically activates a conda environment when
# entering a folder with an environment.yml file.
#
# If the environment doesn't exist, conda-auto-env creates it and
# activates it for you.
#
# To install add this line to your .bashrc or .bash-profile:
#
#       source /path/to/conda_auto_env.sh
#

function conda_auto_env() {
  if [ -e "environment.yml" ]; then
    # echo "environment.yml file found"
​    ENV=$(head -n 1 environment.yml | cut -f2 -d ' ')
    # Check if you are already in the environment
​    if [[ $PATH != *$ENV* ]]; then
      # Check if the environment exists
​      source activate $ENV
​      if [ $? -eq 0 ]; then
​        :
​      else
        # Create the environment and activate
​        echo "Conda env '$ENV' doesn't exist."
​        conda env create -q
​        source activate $ENV
​      fi
​    fi
  fi
}

export PROMPT_COMMAND=conda_auto_env



# Modified from:
# https://github.com/chdoig/conda-auto-env

# Auto activate conda environments
function conda_auto_env() {
  if [ -e "environment.yaml" ]; then
    ENV_NAME=$(head -n 1 environment.yaml | cut -f2 -d ' ')
    # Check if you are already in the environment
​    if [[ $CONDA_PREFIX != *$ENV_NAME* ]]; then
      # Try to activate environment
​      source activate $ENV_NAME &>/dev/null
​    fi
  fi
}

export PROMPT_COMMAND="conda_auto_env;$PROMPT_COMMAND"

