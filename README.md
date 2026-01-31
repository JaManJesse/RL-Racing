Welcome to my github repo for racing experiments with the aerial gym environment

The most important files are racing_task.py, evaluation_task.py and racing_task_config.py

Inside racing_task.py, in reset_idx(), the first part of code is commented out, this is the part necessary for creating models with random tracks. 
Immediately below it, the static track is defined. 

Furthermore, in compute_reward(), the commented part is part of the original navigation task logic, and is necessary for the navigation random and navigation static models.
The code above the comments is the code necessary for the centerline progression method. 

Evaluation_task.py uses the same logic found in racing_task, but it saves the results of each epoch in a csv file for easy use. 
Racing_task_config.py is similar to navigation_task.py, but contains some additional reward parameters. 

To change the resolution of the sensors, you can navigate to config/sensor_config/{which sensor you use} and change the height and width hyperparams of the sensor.
