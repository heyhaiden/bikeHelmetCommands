![Cover Photo](incrementBikeCommand_inferencing/assets/smartHelmet_cover.jpg)

## Introduction
The inspiration for this project came from iterating on [@djdunc's](xxx) gesture detection model for driving a smart helmet. The decision to switch the detection model to audio classification was done in order to get a more consistent result that limited the amount of false positives, and made the experience safer and completely "hands free" for the user.

This system utilizes Edge Impulse to deploy an audio classification model on an Arduino Nano 33 BLE Sense that drives an embedded LED strip for hands free signalling using the keywords **"left"** and **"right"**. 

Multiple experiments were run in order to determine an optimal model trained specifically for outdoor deployment in a noisy environment, with the ability to consistently recognize multiple keywords.

### Edge Impulse Models
- [Single Keyword](https://studio.edgeimpulse.com/studio/198343)
- [Dual Keyword](https://studio.edgeimpulse.com/studio/198602)
- [Incremental Keyword](https://studio.edgeimpulse.com/studio/198643)

## Research Question
This project investigated two questions:

1. Is audio classification detection with a single keyword more accurate than a multi-keyword model?
2. Does incremental training produce a more accurate model overall when using multiple keywords?

## Application Overview
Edge Impulse was the key component for the organization and execution of the project. It enabled easy data ingestion and direct capture using the onboard microphone of the Nano BLE Sense. 

![Edge Impulse Workflow](incrementBikeCommand_inferencing/assets/edgeImpulse_diagram.jpg)
source: [https://www.edgeimpulse.com/blog/getting-started-with-edge-impulse](https://www.edgeimpulse.com/blog/getting-started-with-edge-impulse)

This workflow made it possible for continuous iterations with both data training sets and adjustments to the neural network as well. Once the training and testing was complete, Edge Impulse generated a library for the Arduino IDE in order to easily deploy onto my selected board.


## Data
Describe what data sources you have used and any cleaning, wrangling or organising you have done. Including some examples of the data helps others understand what you have been working with.

*Tip: probably ~200 words and images of what the data 'looks like' are good!*

## Model
This is a Deep Learning project! What model architecture did you use? Did you try different ones? Why did you choose the ones you did?

*Tip: probably ~200 words and a diagram is usually good to describe your model!*

## Experiments
What experiments did you run to test your project? What parameters did you change? How did you measure performance? Did you write any scripts to evaluate performance? Did you use any tools to evaluate performance? Do you have graphs of results? 

*Tip: probably ~300 words and graphs and tables are usually good to convey your results!*

## Results and Observations
Synthesis the main results and observations you made from building the project. Did it work perfectly? Why not? What worked and what didn't? Why? What would you do next if you had more time?  

*Tip: probably ~300 words and remember images and diagrams bring results to life!*

## Bibliography
*If you added any references then add them in here using this format:*

1. Last name, First initial. (Year published). Title. Edition. (Only include the edition if it is not the first edition) City published: Publisher, Page(s). http://google.com

2. Last name, First initial. (Year published). Title. Edition. (Only include the edition if it is not the first edition) City published: Publisher, Page(s). http://google.com

*Tip: we use [https://www.citethisforme.com](https://www.citethisforme.com) to make this task even easier.* 

----

## Declaration of Authorship

I, Haiden McGill, confirm that the work presented in this assessment is my own. Where information has been derived from other sources, I confirm that this has been indicated in the work.


Haiden McGill

24 April 2023
