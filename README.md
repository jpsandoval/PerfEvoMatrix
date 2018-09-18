# Performance Evolution Matrix
This respository contain the artifacts needed to replicate our experiment in the paper "Performance Evalution Matrix".



# Baseline

#### Open Baseline Image.


** MacOSX.** We do all the experiments in a Mac Book Pro. To open the Baselina setup execute the following command in the folder where this project was download.

```
./Pharo-OSX/Pharo.app/Contents/MacOS/Pharo Baseline.image
```

** Windows**
You may also run the experiment in Windows, but depending of the windows version you have installed it may be some some UI bugs.
```
cd Pharo-Windows
Pharo.exe ../Baseline.image
```

** Pharo Image ** After open the Baseline Image you should see the following window:

![BaseLine Image Preview](images/BasePlayground.png?s=100)

#### Before & After Working Session

Before each participant init a task we execute the following script in smalltalk. It allow us to track the time that user init the experiment and how many mouse clicks, movements.
```
UProfiler newSession.
UProfiler current start.
```

After finish the task we executed the following script. It stop recording the mouse events and save the stop time.
```
UProfiler current end.
```

The last script generate a txt file with the following information: start time, end time, number of clicks, number of mouse movements, and number of mouse drags (we do not use this last one).
```
11:34:52.5205 am,11:34:56.38016 am,14,75,0
```

# Matrix


