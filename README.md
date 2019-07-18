# Workshop: Hands-on Introduction to Data Analytics and Machine Learning in Optical Networks,

## Wednesday, 31 July, 12:30-14:00, Bayside Room

### Organizers: Carlos Natalino and Marija Furdek

**Abstract**: In this workshop/tutorial, the audience will be guided through the first steps necessary for applying data analytics and machine learning to optical networks. The workshop will allow attendees to use the available development tools (e.g., Jupyter Lab), enable participants to perform data importing and selection (e.g., removing samples with missing features), as well as explore the correlation between the different features of the dataset. The tutorial will be concluded with an interactive discussion on the remaining challenges and ideas for extensions. Lunch will be included.
 
To find out more about this event, please visit the [Congress website](https://www.osa.org/en-us/meetings/osa_meetings/advanced_photonics_congress/program/special_events/).
 
If you have any questions or concerns, or have any issues accessing the link, please email kmaclure@osa.org directly.

If you have any questions or issues while installing the platform necessary to follow this hands-on tutorial, please email carlos.natalino@chalmers.se directly.

## Setting up the environment

During this tutorial, a set of usefull tools will be introduced to the attendees.

### Installing required software

All the software used in this tutorial is open source and free. As an attendee, you need to install the following software:

* Git ([official download page](https://git-scm.com/downloads))
* Python 3.6 or 3.7 (we recommend the Anaconda distribution with Python 3.7 available [here](https://www.anaconda.com/distribution/)) -- a comprehensive installation tutorial is available [here](https://problemsolvingwithpython.com/01-Orientation/01.03-Installing-Anaconda-on-Windows/)
* NodeJS (available [here](https://nodejs.org/en/download/)) -- **optional** for those who will also install the variable inspector (see below)

After installing these software, you should be able to use the commands `git` and `npm` in your prompt (in Windows) or terminal (in Linux and MacOS).

### Installing Python libraries

Once Anaconda is installed, open the Anaconda prompt (in Windows) or the terminal (in Linux or MacOS) and run the following command line:

```
conda create --name handsontutorial numpy pandas scikit-learn matplotlib seaborn tensorflow keras jupyterlab
```

The above command is responsible for creating an environment named `handsontutorial` and installing the following packages:

* Pandas
* Scikit-Learn
* Matplotlib
* Seaborn
* Keras
* TensorFlow
* NumPy
* Jupyter Lab

### Installing Jupyter Lab Variable Inspector (optional)

During the tutorial, the variable inspector will be used. This installation is optional and the tutorial can be followed without problems without this inspector.

The variable inspector is available [here](https://github.com/lckr/jupyterlab-variableInspector). In the following, the installation procedures available in the official repository are reproduced:

1. Enable the `handsontutorial` environment by typing the following command in your Anaconda prompt (in Windows) or terminal (in Linux and MacOS):

```
conda activate handsontutorial
```

2. Clone the git repository by typing the following command in your prompt (for Windows) or terminal (for Linix and MacOS):

```
git clone https://github.com/lckr/jupyterlab-variableInspector
```

3. Once you downloaded the repository use the following steps:

```
cd jupyterlab-variableInspector
npm install
npm run build 
jupyter labextension install . 
``` 


4. Confirm the installation of the extension with:

```
jupyter labextension list
```

which should print `enabled` and `OK`.