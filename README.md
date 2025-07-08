# Neural-Networks-Activation-Functions-Optimizers-and-Regularization
Mini project to experiment with neural network architecture and evaluate how different activation functions, optimizers, and regularization techniques impact classification accuracy on the SKlearn Iris dataset. 

I. Use Pytorch to create a neural network classifier and experiment with the following architecture: 
* Activation functions:
  1. Rectified Linear Units (ReLu) Activation Function
  2. Identify Activation Function
  3. Sigmoid Activation Function


![Screenshot 2025-07-08 at 11 05 25 AM](https://github.com/user-attachments/assets/93c6bb40-2ae4-4cc3-aeff-e582b3b3cd22)
 
* Optimizers:
  1. Baeline - no optimizer (sigmoid activation function)
  2. Stochastic Gradient Descent (SGD) Optimizer 
  3. Adam Optimizer
  4. Adagrad Optimizer

![Screenshot 2025-07-08 at 11 05 38 AM](https://github.com/user-attachments/assets/52ed78d9-2abf-4482-b9a5-790f79525532)
  

* Regularizations
  1. Baseline (no regularization)
  2. Batch Norm Regularization
  3. Dropout Regularization
  4. Weight Init Regularization
 
  ![Screenshot 2025-07-08 at 11 05 51 AM](https://github.com/user-attachments/assets/d0461f72-6b3b-4b78-bf40-4eebf252f1db)
 

III. Key Findings
The baseline model with a sigmoid activation function and Adagrad optimizer achieved the highest accuracy on the iris dataset, outperforming all other model combinations.

The baseline model with a sigmoid activation and Adam optimizer came close in performance, achieving an accuracy of 93%.

The strong performance of the sigmoid activation function is attributed to the clear class boundaries present in the iris dataset, which is well-suited for this activation type.

Adagrad optimizer proved especially effective on the small iris dataset, slightly outperforming Adam (96% vs 93%), likely due to its adaptability on small to medium datasets.

Both Adagrad and Adam optimizers led to the fastest training times among all models tested (0.0099 seconds and 0.0073 seconds, respectively), thanks to their adaptive learning rates enabling faster convergence.

The model using the SGD optimizer was the second slowest to train, likely due to its fixed learning rate and greater sensitivity to hyperparameter tuning, which can hinder convergence if not optimally set.

The choice of optimizer had a noticeable impact on both accuracy and training time, emphasizing the importance of optimizer selection for small datasets.

IV. Skills Demonstrated
Comparative evaluation of neural network optimizers (Adagrad, Adam, SGD) on a classic multiclass classification problem.

Implementation and tuning of activation functions within neural network architectures.

Analysis of optimizer effects on both model accuracy and training efficiency.

Interpretation of results in the context of dataset characteristics and optimizer properties.

Effective communication of experimental findings through concise reporting and evidence-based reasoning.
