# Orekit Tutorials Environment Setup

This guide explains how to create and activate the `orekit_tutorials_env` environment for running Orekit-based tutorials and related tools.

---

## Prerequisites

1. **Install Anaconda/Miniconda**  
   Ensure you have [Anaconda](https://www.anaconda.com/products/distribution) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed on your system.

2. **Clone or Download the Repository**  
   Clone or download this repository to your local machine.

---

## Steps to Create the Environment

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
