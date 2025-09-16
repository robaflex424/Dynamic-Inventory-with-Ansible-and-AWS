This small project shows how dynamic inventories work

Requirements:
    1. key pair to access the instance
    2. set permissions for key pair
        **chmod 400 {key pair name}**

To use this project for your needs you have to follow these steps

#These instructions are for OS based on debian

1. Install python
    
    sudo apt install python3

2. Create venv

    python3 -m venv ~/your_project_venv
    
3. Activate venv

    source ~/{path to your project venv}/bin/activate

4. Install boto3 and botocore

    pip install boto3 botocore

after that you can run your commands successfully