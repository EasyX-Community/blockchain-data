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
EOF
