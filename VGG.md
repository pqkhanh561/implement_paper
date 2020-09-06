# VGG 16


* The paper recommend small conv uses rather than large one. 
	* Make the decistion function more discriminative (????)
	* Decrease parameter of network


The incorporation of **1x1 conv** is a way to increase the non-linearity of the decision function without affecting the receptive fields of the conv. layers.

==> What is decistion function?

* **Architect**
	* **Dropout layer** is placed after dense (rate=0.5).
	* Batch size: 256
	* L2 penaties: 5.10^-4
	* learning rate: 10^-2 and decrease by a factor 10 when the accuracy of validation stopped improving




##Implement
Know how to create the custom model (need to study about __build__). Need to show summary of custom model 
==> The __build__ mean to really know the input shape. The summary of model can be check by using the Input(shape=(), batch_size) to run first.

The paper had many parameters to control (early stop, learning rate, ...) 
