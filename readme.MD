## Prerequisites

1. **Install Anaconda/Miniconda**  
   Ensure you have [Anaconda](https://www.anaconda.com/products/distribution) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed on your system.

2. **Clone or Download the Repository**  
   Clone or download this repository to your local machine.

## Create the Environment and 

```bash
# Navigate to the directory containing the environment.yml file
cd /path/to/your/repository

# Create the environment
conda env create -f orekit_tutorials_env.yml

# Activate the environment
conda activate orekit_tutorials_env

# Verify the installation
python -c "import orekit; print('Orekit is installed successfully!')"
python -c "import matplotlib, numpy, spacetrack, sp3; print('All packages are imported successfully!')"
```

## Update the Repository Without Overwriting Work
```bash
# Save your current work
# Copy the notebooks you're working on to a separate directory
cp -r orekit_tutorial_1.ipynb my_solutions/orekit_tutorial_1.ipynb
cp -r orekit_tutorial_2.ipynb my_solutions/orekit_tutorial_2.ipynb

# Update the repository with the latest changes
git stash         # Temporarily save your local changes
git pull          # Fetch the latest updates from the repository
git stash pop     # Reapply your saved changes

# Work on the new notebooks
# Check the repository for new tutorials, e.g., orekit_tutorial_3.ipynb
cp -r orekit_tutorial_3.ipynb my_solutions/orekit_tutorial_3.ipynb
```