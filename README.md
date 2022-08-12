 <center><h2><ins>Runst, a project to learn neural network and Rust</ins></h2></center>

As Runst is a big project, I must have a deep understanding of what I am doing and why.
And I learned through my school projects that explaining what I did force me to tackle subjects I skimmed over when I was doing those and have a better understanding of my project.

My goal is to create a module that will make easier the creation of a neural network.

<ins>What is a neural network</ins>
A neural network can be separated in three main area:
<p align="center">
    <img src="nn1.png" width="500"/>
</p>

- Informations relative to what we are looking for are put in the input layer; 
- The hidden layer do all the calculations to get a result with the information put in the input layer;
- The output layer will show the result and compare it to the result that was expected.

Each of those layers have a certain number of nods called neurones who are connected to the neurones of the adjacents layers by what is called weights.

To make the neural network work the neurones in the input layer will send the informations they hold to the neurones in the hidden layer through the weight. But the weight will have an effect on the informations sent, it will multiply it by the value of the weight:

Then the neurones in the hidden layer will make the sum of the informations sent by the neurones of the input layer multiplied by the weights:
<p align="center">
    <img src="nn2.png" width="300"/>
</p>

In this example, the first neurone sends the number 3 through a weight with the value 5, which means that the neurone in the hidden layer will take 3 * 5 = 15.

But, the neurone will also take the information sent by the second neurone of the input layer, 7, with the weight of the value 10, which makes 70.

The neurone will make the sum of 15 and 70 which is 85, the final value that will use the neurone with something called the activation function, a function that will determine the value that will be sent to the neuron of the output layer.

This can be sum up with matrices:
<p align="center">
    <img src="nn3.png" width="250"/>
</p>

Matrices can help us to calculate all the neurones in the hidden layer:


0 explique ce qu'est un réseau de neurone 
1 création des poids 
2 calcule matrice x vecteur 