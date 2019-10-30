# bitcoinfullnode
bitcoin full node document

** Add repository and install bitcoind ** 

sudo apt-get install build-essential

sudo apt-get install libtool autotools-dev autoconf

sudo apt-get install libssl-dev

sudo apt-get install libboost-all-dev

sudo add-apt-repository ppa:bitcoin/bitcoin

sudo apt-get update

sudo apt-get install bitcoind

mkdir ~/.bitcoin/ && cd ~/.bitcoin/

nano bitcoin.conf

** Add config to bitcoin.conf file ** 

rpcuser=yourusername

rpcpassword=your_password

testnet=0 //*try to run test net then change testnet=1 (faster sync to test)*//

rpcport=8332

rpcallowip=127.0.0.1

rpcallowip=192.168.1.119//*your_local_ip*//

server=1



** Start bitcoind ** 


bitcoind --daemon

or

bitcoind &



** If bitcoind is already started ** 


ps -e | grep bitcoin // returns pid

kill -9 (pid)

bitcoind &


** Test bitcoind is running and working **


bitcoin-cli getinfo


https://youtu.be/hmbxPuTmDNE

