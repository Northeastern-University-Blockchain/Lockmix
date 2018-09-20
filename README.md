# LockCoin
We propose Lockcoin, a protocol to facilitate anonymous payments using the Bitcoin digital currency. 
Setting up the operating environment：

# Installation:

btcd https://github.com/btcsuite/btcd/releases

btcwallet https://github.com/btcsuite/btcwallet/releases

GO sdk https://golang.org/dl/

# Getting Started:

run btcd: btcd -u rpcuser -P rpcpass (--testnet --mainnet)

create btcwallet: btcwallet -u rpcuser -P rpcpass --create

run bctwallet: btcwallet -u rpcuser -P rpcpass -d trace

run server.go 

If everything's working correctly, it'll say "listening on port 8082" or something like that and start downloading a lot of blocks. Afterwards, it'll just run. And then you can run the client.go,it will send a quest to the server and receive a response with a long signature at the end.

ps:We use a parallel strategy to simulate multiple users and test the time required to mix coins in different numbers of users. If you don't want user the Multi-threaded mode，you can comment the code in the client.go, Good luck.
