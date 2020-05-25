# NNFL_MainProject
NNFL : Controlled Dropout
[Project Presentation](https://github.com/)

The IEEE paper implemented can be accessed at [Controlled Dropout: a Different Approach to Using Dropout on Deep Neural Network](https://ieeexplore.ieee.org/document/7881693)

---

### Dropout Regularization Technique

Dropout is a regularization method that approximates training a large number of neural networks with different architectures in parallel.
In dropout, neurons are  randomly dropped out of training with a pre- defined probability. ( It is a hyper parameter )
This is done in order to prevent overfitting and reduce the dependence of neurons on one another during training.

A new variation has been proposed for this technique. This variation focuses on intentionally dropping units so as to form a more organized shape to reduce computation time.

---

### Conclusions

![testerr_controlled](/testerror_controlled_dropout.png)

Controlled Dropout

 - Once training is done, controlled dropout gives a generalization similar to the traditional method on the MNIST dataset.
 - Initially the traditional method seemed to converge faster with controlled dropout making random spikes in test error during training.
 - As expected, increasing test size decreased overfitting and thus increased generalization.
 - Time spent per weight update for controlled dropout was considerably lower and hence controlled dropout finished training earlier than the traditional method for an equal number of weight updates.
 
 ---

### Instructions to Run
- Open Google colab and choose "Upload from Github"
- Choose either `Controlled_Dropout.ipynb` or `Traditional_Dropout.ipynb` based on what you want to run and copy paste their link to open it.
- Go to Runtime -> Change Runtime type. Choose 'GPU' from the drop down menu. This is done to finish the training fast.
- Now Run all the cells normally.
