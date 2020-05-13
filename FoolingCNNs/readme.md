This project shows how machine learning models themselves can be attacked.Specifically, we will fool adeep learning model 
forhand-writtendigit classification to misclassify the digit-images.In this project, you will use low-levelTensorFlow constructs 
to build a deep learning model, and perturb input images using the model as a white box.We use TensorFlow but notKeras, since we
 need to implement the attacking algorithms and Keras constructs are not as flexible as TensorFlow’s own computational-graph-aware modules.
The file provides instructions that are self-explanatory, and can be divided into 8steps: 
1.Step 1: Load the MNIST dataset and divide it into training data and test data;
2.Step 2: Build the deep learning model (computational graph) using TensorFlow;
3.Step 3: Train the deep learning model built in Step 2; since we need to evaluate the loss on a validation dataset periodically, you will also see the validation dataset;
4.Step 4: Write the prediction function to use the trained model to label new digit-images;
5.Step 5: Generate adversarial images using the Fast Gradient Sign Method (FGSM)algorithm, where you will observe the misclassification of perturbed digits;
6.Step 6: Walk you through FGSMimplementation in TensorFlow;
7.Step 7: Let you try out Targeted Fast Gradient Sign Method (T-FGSM), a targeted version of FGSM;
8.Step 8: Compare 3 different attacking algorithms