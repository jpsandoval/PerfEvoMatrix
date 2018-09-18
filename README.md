# Performance Evolution Matrix
This respository contain the artifacts needed to replicate our experiment in the paper "Performance Evalution Matrix".



# Baseline

#### Open Baseline Image.

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


