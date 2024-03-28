# FireView: An Image-based Exploration of Prescribed Fire Simulations 

|![application](doc/img/screen_capture.png)|
| ---- |
|*Screen capture of the FireView application.*|

FireView is an application created to explore the results of fire simulations. To use, first install
pycinema module, which will install the python modules and the `cinema` shell command:

```
pip install pycinema
``` 

Then clone this repository, and run the application as follows:

```
cinema path/to/FireView.py [path/to/database] "initial selection" "list of items selected across windows"
```

# Installing FireView as a Cinema script

Cinema scripts can be installed in a common directory and called with a shorthand command
line arguments. Cinema looks for scripts in a user-controllable location defined by the
environment variable `PYCINEMA_SCRIPT_DIR`. Once this location is defined, the `cinema` 
application will search for named scripts there.

To accomplish this, copy the `FireView.py` script to your location. Then in the shell:

```
export PYCINEMA_SCRIPT_DIR=/directory/with/applications

cinema FireView [cinema database] "SELECT * from index LIMIT 100" "[id list of selection]"
```
