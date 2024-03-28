# FireView: An Image-based Exploration of Prescribed Fire Simulations 

|![application](doc/img/screen_capture.png)|
| ---- |
|*Screen capture of the FireView application.*|

FireView is an application created to explore the results of fire simulations. To use, first install
pycinema module, which will install the python modules and the `cinema` shell command:

```
pip install pycinema
``` 

Then clone this repository and copy the `FireView.py` script in a directory of your choice.

```
cinema FireView [path/to/database] "initial selection" "list of items selected across windows"
```

In the shell:

```
export PYCINEMA_SCRIPT_DIR=/directory/with/applications

cinema FireView [cinema database] "SELECT * from index LIMIT 100" "[id list of selection]"
```
