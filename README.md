# Blockchain Data (Hosted on private server)

Below are a few blockchains data for you to download if you need to sync quickly. They are updated weekly on Sunday @ 0000 EST.

- NRG / Energi - https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#energi3-blockchain-data
- PEXA / Pexacoin - https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#pexa-blockchain-data
- PHL / Placeholders - https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#phl-blockchain-data
- TNA / Taonacoin - https://github.com/EasyX-Community/blockchain-data/blob/master/README.md#tna-blockchain-data

# energi3-blockchain-data
Instructions to download and install Energi3 Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> mkdir -p $HOME/energi3-blockchain-data/<br />
> rm -rf $HOME/energi3-blockchain-data/\*.tar.gz\*<br />
> wget -O $HOME/energi3-blockchain-data/energi3-chaindata.backup.tar.gz \\<br />
> https://hn1.easyx.cc/blockchain-data/energi3-chaindata.backup.tar.gz<br />
> sudo service energi3 stop<br />
> rm -rf .energicore3/energi3/chaindata/\*<br />
> tar xvzf energi3-chaindata.backup.tar.gz<br />
> sudo service energi3 start<br />

#### To Export:
> cd $HOME<br />
> mkdir -p $HOME/energi3-blockchain-data/<br />
> rm -rf $HOME/energi3-blockchain-data/\*.tar.gz\*<br />
> sudo service energi3 stop<br />
> tar cvzf $HOME/energi3-blockchain-data/energi3-chaindata.backup.tar.gz .energicore3/energi3/chaindata/\*<br />
> sudo service energi3 start<br />
<br />

# pexa-blockchain-data
Instructions to download and install Pexacoin Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> mkdir -p $HOME/pexa-blockchain-data/<br />
> rm -rf $HOME/pexa-blockchain-data/\*.tar.gz\*<br />
> wget -O $HOME/pexa-blockchain-data/pexa-chaindata.backup.tar.gz \\<br />
> https://hn1.easyx.cc/blockchain-data/pexa-chaindata.backup.tar.gz<br />
> pexa-cli stop<br />
> rm -rf .pexa/blocks/\* .pexa/chainstate/\*<br />
> tar xvzf pexa-chaindata.backup.tar.gz<br />
> pexad -daemon=1 -txindex<br />

#### To Export:
> cd $HOME<br />
> mkdir -p $HOME/pexa-blockchain-data/<br />
> rm -rf $HOME/pexa-blockchain-data/\*.tar.gz\*<br />
> pexa-cli stop<br />
> tar cvzpf $HOME/pexa-blockchain-data/pexa-chaindata.backup.tar.gz \\<br />
> .pexa/energi3/blocks/\* .pexa/energi3/chainstate/\*<br />
> pexad -daemon=1 -txindex<br />
<br />

# phl-blockchain-data
Instructions to download and install Placeholders Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> mkdir -p $HOME/phl-blockchain-data/<br />
> rm -rf $HOME/phl-blockchain-data/\*.tar.gz\*<br />
> wget -O $HOME/phl-blockchain-data/phl-chaindata.backup.tar.gz \\<br />
> https://hn1.easyx.cc/blockchain-data/phl-chaindata.backup.tar.gz<br />
> placehd-cli stop<br />
> rm -rf .placeh/blocks/\* .placeh/chainstate/\*<br />
> tar xvzf phl-chaindata.backup.tar.gz<br />
> placehd -daemon=1 -txindex<br />

#### To Export:
> cd $HOME<br />
> mkdir -p $HOME/phl-blockchain-data/<br />
> rm -rf $HOME/phl-blockchain-data/\*.tar.gz\*<br />
> placeh-cli stop<br />
> tar cvzpf $HOME/phl-blockchain-data/phl-chaindata.backup.tar.gz \\<br />
> .placeh/blocks/\* .placeh/chainstate/\*<br />
> placehd -daemon=1 -txindex<br />
<br />

# tna-blockchain-data
Instructions to download and install Taonacoin Blockchain (hosted on a private server)

#### To import:
> cd $HOME<br />
> mkdir -p $HOME/tna-blockchain-data/<br />
> rm -rf $HOME/tna-blockchain-data/\*.tar.gz\*<br />
> wget -O $HOME/tna-blockchain-data/tna-chaindata.backup.tar.gz \\<br />
> https://hn1.easyx.cc/blockchain-data/tna-chaindata.backup.tar.gz<br />
> taona-cli stop<br />
> rm -rf .taona/blocks/\* .taona/chainstate/\*<br />
> tar xvzf tna-chaindata.backup.tar.gz<br />
> taonad -daemon=1 -txindex<br />

#### To Export:
> cd $HOME<br />
> mkdir -p $HOME/tna-blockchain-data/<br />
> rm -rf $HOME/tna-blockchain-data/\*.tar.gz\*<br />
> taona-cli stop<br />
> tar cvzpf $HOME/tna-blockchain-data/tna-chaindata.backup.tar.gz \\<br />
> .taona/blocks/\* .taona/chainstate/\*<br />
> taonad -daemon=1 -txindex<br />
<br />
EOF
