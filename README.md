# Webmail deployment into a dockerized environment

### Requirements
* ec2 instance created in us-east-1 region using Fedora-Cloud-Base-26-1.5.x86_64-us-east-1-HVM-standard-0 (ami-bb6065ad)
* attached security group with tcp:80 and tcp:22 opened
* private key registered in "aws keypairs" and valid for newly created environment

### Prerequisites
* ansible 2.4

### How to run 
1. git clone https://github.com/aleksandrmironov/equitativa.git
2. cd equitativa
3. ansible-playbook -u fedora -s --private-key=devops-us-east-1 -i '54.163.23.48,' deploy.yml (please replace key and ip address with yours)


