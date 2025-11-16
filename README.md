## Environment Setup

Below are the steps used to prepare the environment on an AWS EC2 (Amazon Linux / SageMaker) instance:

```bash
# Navigate to project directory
ls
pwd
cd /home
ls
cd ec2-user/
ls
cd SageMaker/
ls
cd Finetuning-on-aws/
ls
git status
clear

# Activate Conda environment
source /home/ec2-user/anaconda3/bin/activate python3

# Upgrade build tools
pip install --upgrade pip setuptools wheel
pip install --upgrade cmake
sudo yum install -y gcc gcc-c++ make

# Install specific dependencies
pip install cmake==3.27.0 pyarrow==16.1.0 --no-cache-dir

# Install project requirements
pip install -r ./finetuning/requirements.txt

# Optional: clear pip cache
pip cache purge
