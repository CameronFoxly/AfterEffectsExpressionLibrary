If you need to have a wiggle loop seamlessly, here's a great expression to do just that. Drop it onto an property that you'd want to wiggle and set the frequence, amplitude, and length of the loop to what makes sense for your project. You can also use theComp.duration for the secondsToLoop, if you want it to loop for the lenght of the comp.

```
frequency = 2; // wiggles per second
amplitude = 40; // amount of pixels to wiggle
secondsToLoop = 3; // time to loop in seconds. Change this to thisComp.duration if more appropriate
// --------
t = time % secondsToLoop;
wiggle1 = wiggle(frequency, amplitude, 1, 0.5, t);
wiggle2 = wiggle(frequency, amplitude, 1, 0.5, t - secondsToLoop);
linear(t, 0,  secondsToLoop, wiggle1, wiggle2)
```
