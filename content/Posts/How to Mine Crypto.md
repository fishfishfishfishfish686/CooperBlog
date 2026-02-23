---
title: How to Mine Crypto
date: 2026-02-23
draft: false
---
# Requirements:
Things you will require to set this server up
- A server, not a VM
- Ethernet and ample cooling

# Setup:
You will need to set up the server with a server os such as Ubuntu Server or Debian.

You will then need to download the required packages:
- git
- build-essential
- cmake
- libuv1-dev
- libssl-dev
- libhwloc-dev

**Install Command:**
```
sudo apt install git build-essential cmake libuv1-dev libssl-dev libhwloc-dev
```
# Installation

You will need to clone the git repo:

```
git clone https://github.com/xmrig/xmrig.git
```

After you will need to enter the repo

```
cd xmrig
```

Once inside you will need to make a new directory to build the program

```
mkdir build
```

Don't forget to enter the build directory after creating it

```
cd build
```

Now you will need to build the xmrig program,

```
cmake ..
```

And make it (this will take ~5 minutes)

```
make
```


# Monero Wallet

You can create a Monero wallet by downloading the GUI wallet from their website: https://www.getmonero.org/downloads/
You can then follow the instructions to create your Monero wallet. To get your wallet address you can click on the Account tab on the left and press the "Copy Address to Clipboard Button" next to Primary Account.

# Post-Installation

One you install the program you will need to run a specific command to run it

```
./xmrig -o <mining Pool> -u <Monero Wallet Address> -p <name for miner>
```

For example here is what I would use

```
./xmrig -o gulf.moneroocean.stream:10128 -u <Wallet Address> -p <miner name>
```

You can add in your wallet address and name. Adding a name is optional however I would highly recommend you add one as if you have 2 miners it helps a lot to differentiate the two miners.

Once run it should look like this

![Image Description](/images/Pasted%20image%2020260223174914.png)
(Mine looks different because it has been running for a while)

After you get an accepted share you can look up your Monero by going to: https://moneroocean.stream and put your wallet address in and see how much crypto you are earning and change payout settings.

# Congrats

You have successfully created a Monero miner and assigned it to your wallet.

Happy Mining,
Cooper