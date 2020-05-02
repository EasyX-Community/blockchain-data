# energi3-blockchain-data
Export of the Energi3 Blockchain

#### To import:
> cd $HOME<br />
> mkdir -p $HOME/energi3-blockchain-data/<br />
> rm -rf $HOME/energi3-blockchain-data/\*.tar.gz\*<br />
> git clone https://github.com/leshacat/energi3-blockchain-data $HOME/energi3-blockchain-data/<br />
> cp $HOME/energi3-blockchain-data/\*.tar.gz\* $HOME<br />
> sudo service energi3 stop<br />
> rm -rf .energicore3/energi3/chaindata/\*<br />
> tar xvzf energi3-chaindata.backup.tar.gz.*<br />
> sudo service energi3 start<br />

#### To Export:
> cd $HOME<br />
> mkdir -p $HOME/energi3-blockchain-data/<br />
> rm -rf $HOME/energi3-blockchain-data/\*.tar.gz\*<br />
> sudo service energi3 stop<br />
> tar cvzf - .energicore3/energi3/chaindata/ | split --bytes=90MB - \\<br />
> $HOME/energi3-blockchain-data/energi3-chaindata.backup.tar.gz.<br />
> sudo service energi3 start<br />
<br />
EOF
