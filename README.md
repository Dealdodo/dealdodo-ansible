# Installing 

## Step 1: Generate key
```sh
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

## Step 2: Copy pub key to github
copy the public key
```sh
cat ~/.ssh/id_rsa.pub
```

Add the key to [Github deploy keys](https://github.com/nickhartjes/dealdodo-ansible/settings/keys)


## Step 3: Run the script
```sh
wget -O - https://raw.githubusercontent.com/nickhartjes/dealdodo-ansible/main/bootstrap.sh | bash
```
