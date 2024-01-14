# EmbryoClassificationModel
An AI classification model to classify different Embryo from dataset.

In this project , we are stepping into the domain where artificial intelligence intertwines with reproductive science to foster better outcomes in embryo selection.
Our project is materialized through the "Hung Vuong Hospital Embryo Classification" dataset, a rich source of data aimed at using machine learning for embryo quality classification.
This dataset is organised into training and testing sets, encompassing images of embryos at critical developmental stages - day-3 and day-5.
The training folder is a comprised of embryonic images intended for honing our model, while the test folder holds unseen data, used to evaluate our model’s prowess in real-world scenarios.
Essential to our analysis is a file structure that encapsulates the essential details of each embryonic image, segregated into 'train.csv' and 'test.csv'. These files are our roadmap to understanding the inherent characteristics of the data, thus, paving the path for a well-informed modelling process.
Now, for our model development , we employ a Convolutional Neural Network (CNN), which is a sterling algorithm known for its efficacy in image recognition tasks.
Using CNN we aim on building a robust model capable of discerning the quality of embryos with high precision. The benefits of this algorithm it that it delves deep into the intricacies of embryonic images, identifying patterns that are emblematic of 'good' or 'not good' classifications.

**Goal:**
Our objective is marked by a straightforward yet impactful objective: to accurately classify embryo images as '1' for good or '0' for not good, for both day-3 and day-5 stages. This classification is not just a binary outcome; it's a leap towards enhancing the success rates of in-vitro fertilization procedures, potentially bringing joy to countless families.
Our success metric is straightforward: achieve a high accuracy rate in classifying the test set, thereby demonstrating the model's aptitude in navigating the nuanced landscape of embryo quality assessment.
As we embark on this innovative journey, the fusion of artificial intelligence and reproductive science holds the promise of igniting a new era of medical advancements, making strides towards a future where technology serves at the forefront of nurturing life.


Since the embryo dataset is in jpg image format, the first obvious choice for which model would be suitable and compatible with the dataset would be convolutional neural networks. This is largely due to the effectiveness and efficiency of the CNN model to learn and classify the dataset. As the layers such as convolution, RELU and pooling are effective in learning and extracting 
Significant features from the image. After the feature learning process is complete, the next is the classification phase using layers such as flatten dense to classify the images based on what was learned in the feature learning phase. Therefore the proposed model that will be used in the AI project is CNN. 
With communication from all members of the team, we have suggested creating our own model and comparing each of the models in terms of the metric accuracy. The model that I used is a regular CNN model, Leonardo's model is efficientNetB0 which is a pre-trained model from tensorflow keras and Henil’s model is ResNet50 which again is a pre-trained model from tensorflow keras. More details on the models.

Use the embryo dataset image, learn features that differentiate between good and bad embryo. We have a particular image at a point from the embryo dataset, then we pass that image input into the CNN model and have filters, convolutional layers, pooling, activation function (RELU), learn important features and then classify the images. Main purpose is to classify specific features within the embryo dataset and figure out if it is good or not.
In terms of evaluation of the model for measuring accuracy and error, we extracted metrics such as loss, accuracy, Type I error and Type II error from a training history and returned them in a list.
Then, we plotted these metrics for both training and validation data across different epochs, providing a visual representation of the model’s performance.
Kevin’s model used a confusion matrix as well in terms of identifying the accuracy and error for the model.
