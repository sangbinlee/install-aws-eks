# install-aws-eks
install-aws-eks



# install aws cli
  
  $ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
  $ unzip awscliv2.zip
  $ sudo ./aws/install
  $ $ aws --version
  aws-cli/2.7.33 Python/3.9.11 Linux/5.15.0-1019-aws exe/x86_64.ubuntu.20 prompt/off


# install aws cli in notebook
  root@master:/home/sangbinlee9# aws --version
  aws-cli/2.13.5 Python/3.11.4 Linux/5.19.0-46-generic exe/x86_64.ubuntu.22 prompt/off
  root@master:/home/sangbinlee9#
  
  
  root@worker2:/home/sangbinlee9# aws --version
  aws-cli/2.13.5 Python/3.11.4 Linux/5.19.0-45-generic exe/x86_64.ubuntu.22 prompt/off
  root@worker2:/home/sangbinlee9#


# AWS CLI Configure

  
  root@master:/home/sangbinlee9# aws configure
  AWS Access Key ID [****************WS4X]: AKIAUBSRxxx
  AWS Secret Access Key [****************z62s]: 6wPDRliUUb+LObsxcZtxxx
  Default region name [ap-northeast-2]: ap-northeast-2
  Default output format [None]:
  root@master:/home/sangbinlee9#

  
  root@worker2:/home/sangbinlee9# aws configure
  AWS Access Key ID [None]: AKIAUBSRxxx
  AWS Secret Access Key [None]: 6wPDRliUUb+LObsxcZtxxx
  Default region name [None]: ap-northeast-2
  Default output format [None]:
  



# install eksctl
  
   curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz" | tar xz -C /tmp
   sudo mv /tmp/eksctl /usr/local/bin
   eksctl version
    
    root@master:~# eksctl version
    0.150.0-dev
    root@master:~#
  
    
    root@worker2:~# eksctl version
    0.150.0-dev
    root@worker2:~#

#  https://github.com/eksctl-io/eksctl/blob/main/README.md#installation



# 이건 aws ec2에서 해야되는거 같아서 여기서 멈춤
# 내가 원하는것은 aws 외부 우분투 서버에서 k8s 설치 하고 싶음.....
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
# 
