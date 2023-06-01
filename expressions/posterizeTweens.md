This expression is to change the framerate of a single property of keyframed animation. 
I generally use it to drop the framerate of a single layers animation to 12fps inside of a 24fps comp. 
It acts similarly to the Poserize Time effect, but works for keyframes without having to precomp.
You apply it to whatever property you'd like at a lower framerate. 
Change the `2` to however many frames you want to be held.  

`if(timeToFrames() % 2 > 0){value}else{valueAtTime(time-thisComp.frameDuration)}`

	
