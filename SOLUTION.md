# Lab SolutionLast login: Mon Feb 16 16:29:11 on ttys000
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 create-vpc --cidr-block 10.0.0.0/16 --tag-specifications 'ResourceType=vpc,Tags=[{Key=Name,Value=bootcamp-vpc}]'
zsh: command not found: aws
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 create-vpc --cidr-block 10.0.0.0/16 --tag-specifications 'ResourceType=vpc,Tags=[{Key=Name,Value=bootcamp-vpc}]'
zsh: command not found: aws
ahmeterdogan@Ahmets-MacBook-Pro ~ % ssh -i "bootcamp-week2-key.pem" ec2-user@100.28.222.217
Warning: Identity file bootcamp-week2-key.pem not accessible: No such file or directory.
ec2-user@100.28.222.217: Permission denied (publickey,gssapi-keyex,gssapi-with-mic).
ahmeterdogan@Ahmets-MacBook-Pro ~ % ssh -i ~/Downloads/bootcamp-week2-key.pem ec2-user@100.28.222.217
   ,     #_
   ~\_  ####_        Amazon Linux 2023
  ~~  \_#####\
  ~~     \###|
  ~~       \#/ ___   https://aws.amazon.com/linux/amazon-linux-2023
   ~~       V~' '->
    ~~~         /
      ~~._.   _/
         _/ _/
       _/m/'
Last login: Thu Feb 12 13:44:26 2026 from 46.196.81.56
[ec2-user@ip-172-31-67-153 ~]$ aws ec2 create-vpc --cidr-block 10.0.0.0/16 --tag-specifications 'ResourceType=vpc,Tags=[{Key=Name,Value=bootcamp-vpc}]'

An error occurred (UnauthorizedOperation) when calling the CreateVpc operation: You are not authorized to perform this operation. User: arn:aws:sts::341920718143:assumed-role/ec2-s3-cloudwatch-role/i-0c445758559e14172 is not authorized to perform: ec2:CreateVpc on resource: arn:aws:ec2:us-east-1:341920718143:vpc/* because no identity-based policy allows the ec2:CreateVpc action. Encoded authorization failure message: fARkJbyiExaCLOQuO3wQhKy_dGq_lJr60VxKbFWPZOwXKZUG_S5R9iCKZst_gvx3vzdBUj5W5iC_uh6mUPRuTET4V2HigaelYN6MrxFop1r8ykWCbMAAuhkle_UagkeXVXFhqNQcQK1K3Pl080YBo72AJwpm_iFAKZP8qMJfJ_CeUkCwUF4kiWAH6PK_UsjY_bzV_M9r5oqVqab6XvQXhqaCbZ-4Nv7Fr4nlX9WUxsjWsFMS2ZPcIdY14n8Icl7JUfHyfO1NDr9iFRl1LwW8uQPnvZTUbeb81Uo7K1mAHZquuiE6lL9HnGET6IJc7PzYd2GHBMgciBnU4P-b-arjFbtcAuVBe-a1ZvsjvEzkbd-F7qyfZPz_qO-vxnbgbRnXjM3BsXcsE-Pz48mPaw_9QtQ76VXYQKOY49Ze3YmQsbaFux3Xbe8om4ItxjA3EzH2NCusEPu__lDGs5y2GbcApZ5ePXj2Rb9FaubJN9dmGUz4h4GZ7x3qg7ng9weZG3qNAHayqm71c4KZKT8mQdcqq7LGg7hFPGVXJ6TTiQu7emA_GeSvOxp_
[ec2-user@ip-172-31-67-153 ~]$ Read from remote host 100.28.222.217: Operation timed out
Connection to 100.28.222.217 closed.
client_loop: send disconnect: Broken pipe
ahmeterdogan@Ahmets-MacBook-Pro ~ % 




Last login: Mon Feb 16 19:21:54 on ttys006
ahmeterdogan@Ahmets-MacBook-Pro ~ % ssh-add -K ~/Downloads/Bootcamp-week2-key.pem
WARNING: The -K and -A flags are deprecated and have been replaced
         by the --apple-use-keychain and --apple-load-keychain
         flags, respectively.  To suppress this warning, set the
         environment variable APPLE_SSH_ADD_BEHAVIOR as described in
         the ssh-add(1) manual page.
Identity added: /Users/ahmeterdogan/Downloads/Bootcamp-week2-key.pem (/Users/ahmeterdogan/Downloads/Bootcamp-week2-key.pem)
ahmeterdogan@Ahmets-MacBook-Pro ~ % ssh -A ec2-user@100.28.222.217
   ,     #_
   ~\_  ####_        Amazon Linux 2023
  ~~  \_#####\
  ~~     \###|
  ~~       \#/ ___   https://aws.amazon.com/linux/amazon-linux-2023
   ~~       V~' '->
    ~~~         /
      ~~._.   _/
         _/ _/
       _/m/'
Last login: Mon Feb 16 16:23:39 2026 from 178.230.112.103
[ec2-user@ip-172-31-67-153 ~]$ ssh ec2-user@172.31.14.41
ssh: connect to host 172.31.14.41 port 22: Connection timed out
[ec2-user@ip-172-31-67-153 ~]$ aws ssm start-session --target i-0c445758559e14172

An error occurred (AccessDeniedException) when calling the StartSession operation: User: arn:aws:sts::341920718143:assumed-role/ec2-s3-cloudwatch-role/i-0c445758559e14172 is not authorized to perform: ssm:StartSession on resource: arn:aws:ssm:us-east-1:341920718143:document/SSM-SessionManagerRunShell because no identity-based policy allows the ssm:StartSession action
[ec2-user@ip-172-31-67-153 ~]$ ssh ec2-user@172.31.14.41
exit
^C
[ec2-user@ip-172-31-67-153 ~]$ 
[ec2-user@ip-172-31-67-153 ~]$ 
[ec2-user@ip-172-31-67-153 ~]$ 
[ec2-user@ip-172-31-67-153 ~]$ curl http://checkip.amazonaws.com
^[[A^[[B^[[B^[[B



^X
^C
[ec2-user@ip-172-31-67-153 ~]$ ^C
[ec2-user@ip-172-31-67-153 ~]$ ^C
[ec2-user@ip-172-31-67-153 ~]$ ^C
[ec2-user@ip-172-31-67-153 ~]$ ^C
[ec2-user@ip-172-31-67-153 ~]$ ^C
[ec2-user@ip-172-31-67-153 ~]$ 
[ec2-user@ip-172-31-67-153 ~]$ 
[ec2-user@ip-172-31-67-153 ~]$ 
[ec2-user@ip-172-31-67-153 ~]$ 
[ec2-user@ip-172-31-67-153 ~]$ 
[ec2-user@ip-172-31-67-153 ~]$ curl http://checkip.amazonaws.com
^C
[ec2-user@ip-172-31-67-153 ~]$ 10.0.11.6
-bash: 10.0.11.6: command not found
[ec2-user@ip-172-31-67-153 ~]$ ssh ec2-user@10.0.11.6
ssh: connect to host 10.0.11.6 port 22: Connection timed out
[ec2-user@ip-172-31-67-153 ~]$ ssh ec2-user@10.0.11.6
ssh: connect to host 10.0.11.6 port 22: Connection timed out
[ec2-user@ip-172-31-67-153 ~]$ Read from remote host 100.28.222.217: Operation timed out
Connection to 100.28.222.217 closed.
client_loop: send disconnect: Broken pipe
ahmeterdogan@Ahmets-MacBook-Pro ~ % 


Last login: Mon Feb 16 16:49:15 on ttys000
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 allocate-address --domain vpc
{
    "AllocationId": "eipalloc-09de19d55db559f5a",
    "PublicIpv4Pool": "amazon",
    "NetworkBorderGroup": "us-east-1",
    "Domain": "vpc",
    "PublicIp": "54.164.104.252"
}
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 create-nat-gateway \
  --subnet-id subnet-public-1a \
  --allocation-id eipalloc-xxxxx

An error occurred (InvalidSubnet) when calling the CreateNatGateway operation: The subnet ID 'subnet-public-1a' is malformed
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 describe-subnets --filters "Name=tag:Name,Values=subnet-public-1a" --query "Subnets[*].SubnetId" --output text
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 create-nat-gateway \
  --subnet-id subnet-0aa203880c84bb583 \
  --allocation-id eipalloc-09de19d55db559f5a
{
    "ClientToken": "0e1cdb97-db7f-4eff-a907-06a05bb35350",
    "NatGateway": {
        "CreateTime": "2026-02-16T14:39:33+00:00",
        "NatGatewayAddresses": [
            {
                "AllocationId": "eipalloc-09de19d55db559f5a",
                "IsPrimary": true,
                "Status": "associating"
            }
        ],
        "NatGatewayId": "nat-0cfdf66f09ded801d",
        "State": "pending",
        "SubnetId": "subnet-0aa203880c84bb583",
        "VpcId": "vpc-010ffb449ac8878d0",
        "ConnectivityType": "public",
        "AvailabilityMode": "zonal"
    }
}
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 wait nat-gateway-available --nat-gateway-ids nat-xxxxx

Waiter NatGatewayAvailable failed: An error occurred (NatGatewayMalformed): Invalid Nat Gateway nat-xxxxx
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 wait nat-gateway-available --nat-gateway-ids nat-0cfdf66f09ded801d
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 wait nat-gateway-available --nat-gateway-ids nat-0cfdf66f09ded801d
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 describe-route-tables --filters "Name=tag:Name,Values=*private*" --query "RouteTables[*].RouteTableId" --output text
rtb-0da920160d5e0b952
ahmeterdogan@Ahmets-MacBook-Pro ~ % aws ec2 create-route \
  --route-table-id rtb-0da920160d5e0b952 \    
  --destination-cidr-block 0.0.0.0/0 \
  --nat-gateway-id nat-0cfdf66f09ded801d
{
    "Return": true
}
ahmeterdogan@Ahmets-MacBook-Pro ~ % ssh -A ec2-user@100.49.42.204

ssh: connect to host 100.49.42.204 port 22: Operation timed out
ahmeterdogan@Ahmets-MacBook-Pro ~ % 
ahmeterdogan@Ahmets-MacBook-Pro ~ % ssh -A ec2-user@100.49.42.204
ssh: connect to host 100.49.42.204 port 22: Operation timed out
ahmeterdogan@Ahmets-MacBook-Pro ~ % ssh -A ec2-user@100.49.42.204
ssh: connect to host 100.49.42.204 port 22: Operation timed out
ahmeterdogan@Ahmets-MacBook-Pro ~ % curl http://checkip.amazonaws.com
178.230.112.103
ahmeterdogan@Ahmets-MacBook-Pro ~ % ssh -A ec2-user@100.49.42.204
ssh: connect to host 100.49.42.204 port 22: Operation timed out
ahmeterdogan@Ahmets-MacBook-Pro ~ % 


