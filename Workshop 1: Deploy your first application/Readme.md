# Prerequisite

Follow the [Environment](https://github.com/xuyuji9000/aws-playground#environment-preparation) get yourself prepared for the workshop

# Workflows



## local docker workflow

1. Build Docker image:

    ```bash
    pushd node-playground
    docker build -t node-playground .
    popd
    ```

2. Run Docker container:

    ```bash
    docker run -d -p 8000:8000 node-playground
    ```

3. Check your application

    ```bash
    open http://localhost:8000
    ```

## vanilla elastic beanstalk workflow

1. Create Elastic Beanstalk application

    ```bash
    eb init
    ```

2. Create Environment

    ```bash
    eb create
    ```

3. Deploy application

    ```bash
    eb deploy
    ```

## IaC powered workflow


1. init local terraform working environment

    ```bash
    terraform init
    ```

2. Review stack creation plan

    ```bash
    terraform plan
    ```

3. Create stack

    ```bash
    terraform apply
    ```


4. Connect to  Elastic Beanstalk application and environment

    ```bash
    eb init
    ```
5. Deploy application

    ```bash
    eb deploy
    ```
    
    USEFUL LINKS:
     ```bash
    Getting started on Terraform: https://www.terraform.io/intro/getting-started/install.html
    ```
    ```bash
    Getting Started on Docker: https://runnable.com/docker/install-docker-on-linux
    ```
    
