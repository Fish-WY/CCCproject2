# Introduction of Twitter Harversters
## runSearch.py
start the harverster using searchAPI

```
nohup python3 ~/CCCproject2-team56/TwitterHarverster/runSearch.py > searchout.txt &
```
## runStream.py
start the harverster using streamAPI

```
sudo nohup python3 /home/ubuntu/CCCproject2-team56/TwitterHarverster/runStream.py 0 1 > streamout.txt 2 > streamerr.txt &
```
## command to monitor and kill process
```
ps -ef | grep .py
kill [NO]
```
## CouchDBtools.py & TwitterAPItools.py
defined python functions for couchDB and Twitter API to be called by run*.py

## docReader.py
read and process downloaded historic tweets from UNIMELB cloud
```
./cloudDataProcesser.sh 
# python3 docReader.py 1>/dev/null 2>error.txt &
# nohup python3 docReader.py 1>docout.txt 2>docerror.txt &
```
## APIconfig.py
metadata such as carBrands, coordinations ......
## dependency
```
pip3 install cloudant
pip3 install geotext
pip3 install vaderSentiment
pip3 install tweepy
pip3 install pprint
```
