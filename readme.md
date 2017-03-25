# Scabbard Project Proposal

## Background

Female-presenting internet denizens commonly have to deal with a continuous influx of undesired images of male genitalia on any website that allows interuser interaction, spanning social networks like Facebook and Twitter and Snapchat to dating sites like Tinder and OkCupid. The images are not sent in aspiration of sex, but more realistically as a means of forcing themself into the space of the recipient, demanding their attention and time, even if only to be blocked, reported, and banned. Unwanted dick pics are one member of a more general form of harassment and bullying by the sending of images the sender expects with upset the recipient including, for example, sending nazi imagery to jewish people, extreme gore from their apartheid to pro-palestinian activists, and mutilated fetuses to pregnant women considering or planning abortion.

Despite immense advances in image recognition in recent years, the common response accross all major technosocial platforms has been a complete failure to address the problem preemptively, at best banning the senders. Commonly recipients are left with requesting help from police, who fail to address the problem because they don't understand the tech, the sender's location is unknown, or it is ostensibly not their jurisdiction.

## Objective 

Recognize likely-undesired images and enforce good consent practices by covering it while providing an option to view it regardless.

## High Level Requirements

### Minimum Requirements:
1. *Automatic:* If the user needs to trigger filtering manually, it has failed.
1. *Consent-Respecting:* Not all dicks are undesired. The user must be aware the image is covered and for what reason, and be able to see the original image easily.
1. *Better than a Dick Pic:* Whatever the image is covered with, it should be materially better to experience than a dick pic. This may be more complicated than it would seem at first glance.
1. *Specificity:* Categorical misclassification problems, such as labeling all root vegetables as dicks or white men as Hitler, would significantly decrease trustworthiness of the tool.

### Basic Requirements:
1. *Universal:* If filtering is only applied on Tumblr but not OkCupid, that's a start, but better is achievable.
1. *Nonshaming:* If pictures are recieved consensually, overeagerly labeling the sender as toxic is unlikely to be recieved well. We're not in the buisness of preventing the discussion of difficult or sexual topics- the goal is simply to structurally enforce the respect of consent into the conversations taking place.
1. *Individual Modular Configurability:* Not all types of images commonly used in harassing nonconsenting recipients will be unacceptable to everybody. A remotely-consulting surgeon will likely want to disable a gore filter, a sex education specialist will likely want to disable the dick filter; these categorical decisions should be easy to enter, presented to the user when relevant, and easily respected.
1. *Longevity:* Have a plan in place for how the tool can continue to be relevant and useful after your project is over.

### Ideal Capabilities:
1. *Noninvasive:* Ideally only the image would be covered.
1. *Extensibility:* As new categories and forms of harassment come up, new categories should be easily added.
1. *Video:* If all it takes to guarantee reception is using a video or gif instead of a picture, the tool is easily circumvented
1. *Reporting Incorrectly-classified Images for Universal Retraining:* Users should be able to report incorrectly labeled images as their correct categories, and the associated information should be collected and used to retrain the models, as long as the user expresses approval on a granular level.
1. *API for other organizations to report images for global retraining:* Most major social networks have moderation teams of some kind to label images as obscene or harrasment. Might as well make it easy for them to pass those images our way for retraining of the model.
1. *Easy redistribution of pretrained recognizers:* When a model is retrained, the users with the tool already installed should recieve the updates.
1. *Open-source All the Way Down:* The goal is to provide a service by making the world suck less. This is best achieved by facilitating others' use of the models we provide; this way it might see use in ways, hardware, or environments we never imagined it being used in. Open-sourcing the tool is also crucial to facilitate trust that the app is not deceitfully sending all screencaps somewhere or something similarly nefarious.


## Ethics/Social Justice Concerns

+ This project toes a fine line between overaggressive sexshaming and permissive facilitating of aggressors. Care must be taken to respect the significance of images that, despite triggering this tool's classifier, have broader cultural significance, often referred to as iconic. Handling this will require nuance.
+ Note that because of the background and identity of the project proposer, this proposal indubitably fails to account for a multitude of forms or harassment. No list I have provided is complete; it's of the utmost importance that the tool is accounting for needs as broadly as possible rather than merely those I or the engineers of the project are aware of off the tops of our heads. This will require actively seeking out the problems faced by and perspective of people unlike you.

## Provided Materials & Recommended Research Topics

+ Possibly relevant materials include Yahoo's open-nsfw.
+ I personally find the idea of gifs like [this](resources/rainingmen.gif) from [this fantastic music video](https://www.youtube.com/watch?v=l5aZJBLAu1E) as covers to be particularly suitable, but recommend getting the perspective of anybody aside from me.
+ Look into examples of ways past attempts to use AI across a broad spectrum of appearances have gone poorly- often called 'algorithmic racism' and 'biases in learned models'. Also look into efforts to create more diverse training sets to prevent algorithmized unjustice due to data biases. Much discussion has explored surrounding topics, you're likely to find plenty of analysis to help guide your design and inform your future work.

## Questions for Reflection

+ Why has this problem gone unaddressed for at least half a decade? What unspoken assumptions underlie the failure to address this problem via technical means? What methods were being used to address the problem at all, and what populations did those methods place the most work on?
+ How might a more diverse software engineering community, particularly in higher management levels, have driven higher prioritization of this problem?