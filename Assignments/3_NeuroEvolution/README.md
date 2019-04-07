# Neuroevolution Homework
Now that you've all evolved small neural networks for robots in the worksheets we've explored in class, it's time to coevolved some predator and prey robots using larger brains! The worksheet I've provided shows you how to hookup the robot's camera to a brain, and how to have two populations that you measure fitness on at the same time (i.e., with two robots in an arena at once). The code already has boilerplate evolutionary functionality, but there is plenty of room for improvement or experimentation! 

### Some ideas of places to improve:
1. Improve what the robot gets as input from the camera. Right now it's just the red channel flattened into one long array. What might you do to include information from all three channels?
2. Consider starting with a hand-written prey robot, and evolve a predator (or vice versa). Then use the evolved predator to evolve a better prey brain.
3. Use a 2D representation of neurons to better match the structure of the image input the robot is getting. How might neurons from similar locations in the vision field be connected to hidden layers to maximize the amount of "spatial information"? 
4. Since your robot brain has (many) thousands of weights now, maybe using an indirect encoding (like we discussed with NEAT) to reduce the degrees of freedom you're trying to evolve would help. 
5. How might you implement something like Novelty Search in this environment?

## Rough Rubric
- 5/10 - A couple of simple modifications, like better mutations or fitness evaluations.
- 8/10 - One medium sized modification, like stepwise coevolution -- where you evolve the predators first, then the prey.
- 10/10 - One large sized modification, like implementing Novelty Search, changing the way the brain gets the camera input (e.g., Convolution, 2D Networks), or using an indirect encoding to paint the weights of the brain.
