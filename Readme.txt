# Make a new directory (out of the git repository) for e.g.:
mkdir ../python_virtual_env
# copy stable_requirements.txt into the new directory
cp stable_requirements.txt ../python_virtual_env
# Navigate to the new directory
cd ../python_virtual_env
# Create a python virtual environment named <myVenv>
python3 -m venv myVenv
# Activate the python virtual environment
source myVenv/bin/activate
# Install the required packages
pip3 install -r stable_requirements.txt
# if needed update the stable_requirements.txt by the following command (e.g., after installing a new package or updating and existing one)
pip3 freeze > stable_requirements.txt

