# VALD-Nordbord-Processing
This code was used to derive metrics not produced by Vald that could be of interest for sport scientists. 

Vald Nordbord data that is presented in the Vald Hub provides: impulse for all reps, max force for all reps, torque for all reps, and asymmetry between max forces. 

This code was designed to use the raw force trace data from each session to derive these metrics and more for each repetition.

The code requires force trace data in a .csv file with three columns: 'Time,' 'Left Force,' & 'Right Force.'
  'Time' should be setup to be in 1/50 increments for a normal 50hz sample rate or whatever sample rate the data was captured on. (This can be edited)

This code will provide you a .csv file with all of the data for each repetition based on a specific repetition force threshold of 100N. (This can be edited)

Repetitions begin when force goes higher than 25N and ends when force goes under 25N. (This can be edited)

The final .csv file will have max force, impulse 0.2 seconds, impulse to max force, & time to max force for each side & asymmetry of each repetition based on max force of each repetition. +

There is an optional kernel provided with bar plots of data measures for vizualisation. 

