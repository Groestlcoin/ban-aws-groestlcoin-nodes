# Ban Groestlcoin nodes that are using AWS IP addresses
Script to ban all Amazon Web Services IP address ranges.
Protect your node's ressources from VPS nodes.

The list of AWS IP ranges is obtained from http://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html

## Requirements for the bash script (ban.sh)

### Command-line JSON processor jq.

Install on Debian-based Linux
````
sudo apt-get install jq
````

## Download and use the script

`git clone https://github.com/Groestlcoin/ban-aws-groestlcoin-nodes.git`

Run:

````
cd ban-aws-groestlcoin-nodes   
chmod u+x ban.sh   
./ban.sh
````

### To view banned IP addresses:

````
groestlcoin-cli listbanned
````

### To clear banned IP addresses:

````
groestlcoin-cli clearbanned
````
