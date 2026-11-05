# aws cli install ubuntu



Need to create IAM users first.


aws cli install ubuntu
-----------------------
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install

-> aws configure
    access-key
    screate-key
    us-east-1
    enter

Clean Up Files
-----------------
Remove the downloaded zip file and extracted directory to free up space:
rm -rf awscliv2.zip aws/


ami-0055977a6e828a4f4

aws ec2 run-instances \
    --image-id ami-0055977a6e828a4f4 \
    --instance-type t3.micro \
    --security-group-ids sg-0b09cb8469e721057 \
--tag-specifications 'ResourceType=instance,Tags=[{Key=Name,Value=ansible}]'




