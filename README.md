# WEYC
![WEYC Logo](https://reex.ccore.online/images/coins_custom/reex_45.png)<br>

What is WeyCash (WEYC)?

WeyCash is a peer-to-peer decentralized digital currency for ordinary people, easy to use and acquire. We’re pushing for blockchain mass adoption through Memeification. A sustainable and scalable solution in the content creation sectors on the Blockchain. WeyCash summarizes the best characteristics of digital currencies, which were issued earlier (Bitcoin, Dash, PIVX), such as: increased security, fast consensus mechanism, and increased decentralization achieved by requiring miners to prove the knowledge of the transaction data. The community has created a coin with faster transaction, more secure, masternode and low transaction fee.

WeyCash is a fork of Pivx, improved with some of the following features: 

- DNS hardcoded 
- Consesus by masternode 
- POS 3.0
- Fast transactions featuring guaranteed zero confirmation transaction: Instantsend 
- Intregated BIP38, multisignature, blockexplorer, wallet repair and multisend functions in wallet
- Low transaction fee

WeyCash’s Use-cases:
- Help MEME creators to get tips using WEYC. 
- Provide an online marketplace for content creators. 

WeyCash Specifications:
- Coin Name: WeyCash
- Ticker: WEYC
- Type: POS + Masternode
- Block time 60 seconds
- Block size 3 MB
- Block Reward fluctuates
- Algorithm Quark (pow first 200 blocks)
- Transaction confirmation: 16 blocks
- Min Stake: 6 hours
- Max Supply: 21 Million
- Swap Supply: 1 Million
- Premined amount: 240.000 WEYC (0.11% approx)
- Masternode Collateral: 15.000 WEYC
- Reward: 90% masternode, 10% POS

WeyCash Rewards:

POS Rewards:
```
	     1> block <= 50.000:   2 WEYC
 	50.000> block  <= 100.000: 3 WEYC
        100.000> block <= 150.000: 4 WEYC
	150.000> block <= 200.000: 5 WEYC
	200.000> block <= 250.000: 6 WEYC
	250.000> block <= 300.000: 7 WEYC
	300.000> block <= 350.000: 8 WEYC
	350.000> block <= 400.000: 9 WEYC
	400.000> block <= 450.000: 10 WEYC
	450.000> block <= 500.000: 11 WEYC
	500.000> block <= 550.000: 12 WEYC
	550.000> block <= 600.000: 11 WEYC
	600.000> block <= 650.000: 10 WEYC
 	650.000> block <= 700.000: 9 WEYC
	700.000> block <= 750.000: 8 WEYC
	750.000> block <= 800.000: 7 WEYC
	800.000> block <= 850.000: 6 WEYC
	850.000> block <= 900.000: 5 WEYC
	900.000> block <= 950.000: 4 WEYC
	950.000> block: 2 WEYC
```

Masternode Governance: 

```
   	      0> block <= 200: 0.10% //Preparing last pow block
	    200> block <= 50.000:  0.70%
 	50.000> block  <= 100.000: 0.71%
        100.000> block <= 150.000: 0.73%
	150.000> block <= 200.000: 0.73%
	200.000> block <= 250.000: 0.74%
	250.000> block <= 300.000: 0.75%
	300.000> block <= 350.000: 0.76%
	350.000> block <= 400.000: 0.77%
	400.000> block <= 450.000: 0.78%
	450.000> block <= 500.000: 0.79%
	500.000> block <= 550.000: 0.80%
	550.000> block <= 600.000: 0.81%
	600.000> block <= 650.000: 0.82%
 	650.000> block <= 700.000: 0.83%
	700.000> block <= 750.000: 0.84%
	750.000> block <= 800.000: 0.85%
	800.000> block <= 850.000: 0.86%
	850.000> block <= 900.000: 0.87%
	900.000> block <= 950.000: 0.88%
	950.000> block:	0.90%

```
# Debian/Ubuntu Linux Daemon Build Instructions

```
git clone https://github.com/weycash-project/weycash.git
cd weycash
./autogen.sh
./configure --disable-tests
make -j2 (2 can changed for number os Cpus that have VPS)
cd src
strip weycashd weycash-cli
./weycashd -daemon
```