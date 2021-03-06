# Step 5 - Create a SSH Key Pair

1. Open a new browser tab and navigate to
https://docs.aws.amazon.com/cli/latest/userguide/cli-services-ec2-keypairs.html#creating-a-key-pair
This is the reference for how to use the AWS CLI to create a SSH Key Pair.

2. Navigate back to the CloudShell and click in the terminal to plant your curser.
3. Paste in the following command:
`aws ec2 create-key-pair --key-name cloud_workstation --query 'KeyMaterial' --output text > ~/cloud_workstation.pem`
4. Type `ls -als ~/cloud_workstation.pem` to see the new file with its permissions.
5. Type `chmod 400 ~/cloud_workstation.pem` to change them so that the SSH client does
not throw an error.
6. Rerun `ls -als ~/cloud_workstation.pem` to see the new permissions on the PEM file.
7. Type `cat ~/cloud_workstation.pem` to view the contents of the PEM file.
8. Copy the contents of the PEM file to a file saved somewhere besides the CloudShell
to back it up.

**[Watch the Video](https://youtu.be/_t82air0vss)**
