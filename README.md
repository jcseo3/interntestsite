# Instructions

Create a Packer image of an AWS (Amazon Web Services) website that says "Hello World!". First, download the test.json from this github repository and place it in a local directory along with a json file containing your key variables (i.e., access key and secret key from AWS). Run the following command in your terminal (assuming your json file of key variables is called "keyvariables.json"):

packer build -var-file=keyvariables.json test.json

This command builds your packer image. Log onto your account in AWS and find the AMI you just created through the previous command. Use that AMI to launch an instance on AWS (be sure to edit security settings on the instance to include http and https). Once the instance has been launched, copy and paste the public DNS or IP address into a new web browser and you should see "Hello World!"


#Further

To reflect any updates on the repo, go to the terminal, connect to your instance and git pull origin from /home/interntestsite
