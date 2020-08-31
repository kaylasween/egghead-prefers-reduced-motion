# This code relates to an Egghead video lesson!  

We have three animating sections: one in the header and one for each of the two images. To honor the system preferences of the user, we can use the prefers-reduced-motion media query to turn off those animations. In this example, we'll change the animation-duration of the stretch, spin, and bounce classes to 0.01ms. This will allow us to effectively remove the animations without disrupting any events that are watching for animationend. If you use the transition property, you could add transition-duration: 0.01ms to ensure the transitionend event isn't disrupted as well.

You can certainly stop there, but today, I don't want to completely remove all animation from the page. To add a less-obtrusive animation, we can rename the animation. In this example, we'll rename the stretch animation to pulse and allow that to move from half opacity to full opacity over 1.5 seconds.

It's worth noting that the prefers-reduced-motion media query is not compatible with Internet Explorer. If you support Internet Explorer, please consider removing animations that are prone to disrupt those with vestibular disorders and learning disabilities. If you're not sure if an animation would be distressing to someone, it's best to turn it off.
