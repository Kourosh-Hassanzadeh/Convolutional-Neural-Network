The dataset is Oxford Flowers but it has splitted into two datasets: A and B. A has 4617 samples for train and 1538 samples for test. B has 100 samples for train and 20 samples for test and test_all is 2056 samples from both A and B.
Train a CNN on dataset A. then train on dataset B which is much smaller than A with three different ways:
<ol>
  <li>
    Copying all layers from the previous model that trained on A and just add 20 neurons which are associated with 20 classes of dataset B then train this new network. 
  </li>
  <li>
    Copying all layers from the previous model that trained on A and Freezing all layers except the last layer which is fully connected and just add 20 neurons to the last fc layer and train only the last layer.
  </li>
  <li>
    Copying all layers from the previous model that trained on A and Freezing all layers except the last layer and also freezing 80 neurons of the last fc layer which are associated with 80 classes of dataset A and just add 20 neurons to the last fc layer and train only these 20 neurons.
  </li>
</ol>

You can check the results in document that we prepared. I'm trying to translate it to English.
