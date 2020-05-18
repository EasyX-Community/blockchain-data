# Blockchain Data

Below are a few blockchains data for you to download if you need to sync quickly. If the walletd is able to I have enabled `-txindex -addressindex` for those who need the transaction index as well. They are hosted on a private server and are updated weekly on Sunday @ 0000 EST.

**All downloads are located here:**<br />
DOWNLOADS TEMPORARILY DOWN! MOVING FILES BETWEEN SERVERS.<br />
Main HTTP: http://hn1.easyx.cc:8081/blockchain-data/<br />
Backup HTTPS: https://hn1.easyx.cc/blockchain-data/

**Note:** If the download file is not found or you see a DO_NOT_XFER file inside the directory it means the blockchains are being updated and you should wait until this file disappears.

**Note:** There will be Windows instructions soon. These same files can be extracted into a new folder and copied to your %APPDATA%/CoinName/ directory.

- [NRG / Energi Blockchain Download](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#energi3-blockchain-data "Energi Blockchain Download")
- [PEXA / Pexacoin Blockchain Download](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#pexa-blockchain-data "Pexacoin Blockchain Download")
- [BITC / BitCash Blockchain Download](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#bitc-blockchain-data "BitCash Blockchain Download")
- [PHL / Placeholders Blockchain Download](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#phl-blockchain-data "Placeholders Blockchain Download")
- [TNA / Taonacoin Blockchain Download](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#tna-blockchain-data "Taonacoin Blockchain Download")
- [MALW / Malwarechain Blockchain Download](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#malw-blockchain-data "Malwarechain Blockchain Download")
- [XZC / ZCoin Blockchain Download](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#xzc-blockchain-data "ZCoin Blockchain Download")

 ~ MooCat

# energi3-blockchain-data
Instructions to download and install Energi3 Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> rm -rf $HOME/energi3-chaindata.backup.tar.gz<br />
> wget https://hn1.easyx.cc/blockchain-data/energi3-chaindata.backup.tar.gz<br />
> sudo service energi3 stop<br />
> rm -rf .energicore3/energi3/chaindata/\*<br />
> tar xvzf energi3-chaindata.backup.tar.gz<br />
> sudo service energi3 start<br />

#### To Export:
> cd $HOME<br />
> rm -rf $HOME/energi3-chaindata.backup.tar.gz<br />
> sudo service energi3 stop<br />
> tar cvzf $HOME/energi3-chaindata.backup.tar.gz .energicore3/energi3/chaindata/\*<br />
> sudo service energi3 start<br />

[Back to top](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#blockchain-data "Back to top")

# pexa-blockchain-data
Instructions to download and install Pexacoin Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> rm -rf $HOME/pexa-chaindata.backup.tar.gz<br />
> wget https://hn1.easyx.cc/blockchain-data/pexa-chaindata.backup.tar.gz<br />
> pexa-cli stop<br />
> rm -rf .pexa/blocks/\* .pexa/blocks/index/\* .pexa/chainstate/\*<br />
> tar xvzf pexa-chaindata.backup.tar.gz<br />
> pexad -daemon=1 -txindex -addressindex<br />

#### To Export:
> cd $HOME<br />
> rm -rf $HOME/pexa-chaindata.backup.tar.gz<br />
> pexa-cli stop<br />
> tar cvzpf $HOME/pexa-chaindata.backup.tar.gz \\<br />
> .pexa/blocks/ .pexa/chainstate/<br />
> pexad -daemon=1 -txindex -addressindex<br />

[Back to top](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#blockchain-data "Back to top")

# bitc-blockchain-data
Instructions to download and install BitCash Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> rm -rf $HOME/bitc-chaindata.backup.tar.gz<br />
> wget https://www.easyx.cc/blockchain-data/bitc-chaindata-backup.tar.gz<br />
> bitcash-cli stop<br />
> rm -rf .bitcash/blocks/\* .bitcash/blocks/index/\* .bitcash/chainstate/\*<br />
> tar xvzf bitc-chaindata.backup.tar.gz<br />
> bitcashd -daemon=1 -txindex -addressindex<br />

#### To Export:
> cd $HOME<br />
> rm -rf $HOME/bitc-chaindata.backup.tar.gz<br />
> bitcash-cli stop<br />
> tar cvzpf $HOME/bitc-chaindata.backup.tar.gz \\<br />
> .bitcash/blocks/ .bitcash/chainstate/<br />
> bitcashd -daemon=1 -txindex -addressindex<br />

[Back to top](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#blockchain-data "Back to top")

# phl-blockchain-data
Instructions to download and install Placeholders Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> rm -rf $HOME/phl-chaindata.backup.tar.gz<br />
> wget https://hn1.easyx.cc/blockchain-data/phl-chaindata.backup.tar.gz<br />
> placeh-cli stop<br />
> rm -rf .placeh/blocks/\* .placeh/blocks/index/\* .placeh/chainstate/\*<br />
> tar xvzf phl-chaindata.backup.tar.gz<br />
> placehd -daemon=1 -txindex -addressindex<br />

#### To Export:
> cd $HOME<br />
> rm -rf $HOME/phl-chaindata.backup.tar.gz<br />
> placeh-cli stop<br />
> tar cvzpf $HOME/phl-chaindata.backup.tar.gz \\<br />
> .placeh/blocks/ .placeh/chainstate/<br />
> placehd -daemon=1 -txindex -addressindex<br />

[Back to top](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#blockchain-data "Back to top")

# tna-blockchain-data
Instructions to download and install Taonacoin Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> rm -rf $HOME/tna-chaindata.backup.tar.gz<br />
> wget https://hn1.easyx.cc/blockchain-data/tna-chaindata.backup.tar.gz<br />
> taona-cli stop<br />
> rm -rf .taona/blocks/\* .taona/blocks/index/\* .taona/chainstate/\*<br />
> tar xvzf tna-chaindata.backup.tar.gz<br />
> taonad -daemon=1 -txindex -addressindex<br />

#### To Export:
> cd $HOME<br />
> rm -rf $HOME/tna-chaindata.backup.tar.gz<br />
> taona-cli stop<br />
> tar cvzpf $HOME/tna-chaindata.backup.tar.gz \\<br />
> .taona/blocks/ .taona/chainstate/<br />
> taonad -daemon=1 -txindex -addressindex<br />

[Back to top](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#blockchain-data "Back to top")

# malw-blockchain-data
Instructions to download and install Malwarechain Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> rm -rf $HOME/malw-chaindata.backup.tar.gz<br />
> wget https://hn1.easyx.cc/blockchain-data/malw-chaindata.backup.tar.gz<br />
> malwarechain-cli stop<br />
> rm -rf .malwarechain/blocks/\* .malwarechain/blocks/index/\* .malwarechain/chainstate/\*<br />
> tar xvzf malw-chaindata.backup.tar.gz<br />
> malwarechaind -daemon=1 -txindex -addressindex<br />

#### To Export:
> cd $HOME<br />
> rm -rf $HOME/malw-chaindata.backup.tar.gz<br />
> malwarechain-cli stop<br />
> tar cvzpf $HOME/malw-chaindata.backup.tar.gz \\<br />
> .malwarechain/blocks/ .malwarechain/chainstate/<br />
> malwarechaind -daemon=1 -txindex -addressindex<br />

[Back to top](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#blockchain-data "Back to top")

# xzc-blockchain-data
Instructions to download and install ZCoin Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> rm -rf $HOME/xzc-chaindata.backup.tar.gz<br />
> wget https://hn1.easyx.cc/blockchain-data/xzc-chaindata.backup.tar.gz<br />
> zcoin-cli stop<br />
> rm -rf .zcoin/blocks/\* .zcoin/blocks/index/\* .zcoin/chainstate/\*<br />
> tar xvzf xzc-chaindata.backup.tar.gz<br />
> zcoind -daemon=1 -txindex -addressindex<br />

#### To Export:
> cd $HOME<br />
> rm -rf $HOME/xzc-chaindata.backup.tar.gz<br />
> zcoin-cli stop<br />
> tar cvzpf $HOME/xzc-chaindata.backup.tar.gz \\<br />
> .zcoin/blocks/ .zcoin/chainstate/<br />
> zcoind -daemon=1 -txindex -addressindex<br />

[Back to top](https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#blockchain-data "Back to top")

EOF
