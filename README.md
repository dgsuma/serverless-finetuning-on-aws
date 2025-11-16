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
    Activate the env:
    source /home/ec2-user/anaconda3/bin/activate python3
    pip install --upgrade pip setuptools wheel
    pip install --upgrade cmake
    sudo yum install -y gcc gcc-c++ make
    pip install cmake==3.27.0 pyarrow==16.1.0 --no-cache-dir
    pip install -r ./finetuning/requirements.txt
    pip cache purge
