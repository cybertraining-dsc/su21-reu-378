---
date: 2021-06-16
title: "Project: Detection of Autism Spectrum Disorder with a Facial Image using Artificial Intelligence"
linkTitle: Autism
tags: ["project", "reu","AI",Autism Spectrum Disorder"]
description: "Autism affects 1 in every 160 children worlwide. Early detection and diagnosis of Autism, along with treatment, is needed to minimize some of the difficulties that people with Autism encounter. Autism is usually diagnosed by a specialist through various Autism screening methnods. This can be an expensive and complex process. Many children that display signs of Autism go undiagnosed because there families lack the expenses needed to pay for Autism screening and diagnosing. Therefore, the development of a potential inexpensive, but accurate way to detect Autism in children is necessary for low-income families. With all the technological advances in Artificial Intelligence today, deep learning can be used to develop an effective method to detect Autism in children. This project utilizes a Convolutional Neural Network classifier to explore the possibility of using a facial image analysis to detect Autism in children. The facial images of Autistic and non-autistic male and female children will be used in this project."
author: Myra Saunders
github_url: https://github.com/cybertraining-dsc/su21-reu-378/edit/main/project/index.md
resources:
- src: "**.{png,jpg}"
  title: "Image #:counter"
---

[![Check Report](https://github.com/cybertraining-dsc/su21-reu-378/workflows/Check%20Report/badge.svg)](https://github.com/cybertraining-dsc/su21-reu-378/actions)
[![Status](https://github.com/cybertraining-dsc/su21-reu-378/workflows/Status/badge.svg)](https://github.com/cybertraining-dsc/su21-reu-378/actions)
Status: draft, Type: Project


Myra Saunders, [su21-reu-378](https://github.com/cybertraining-dsc/su21-reu-378), [Edit](https://github.com/cybertraining-dsc/su21-reu-378/blob/main/project/index.md)

* Utilized CNN Code: [autism_classification.ipynb](https://github.com/cybertraining-dsc/su21-reu-378/blob/main/project/code/autism_classification.ipynb)

{{% pageinfo %}}

## Abstract

Autism affects 1 in every 160 children worlwide. Early detection and diagnosis of Autism, along with treatment, is needed to minimize some of the difficulties that people with Autism encounter. Autism is usually diagnosed by a specialist through various Autism screening methnods. This can be an expensive and complex process. Many children that display signs of Autism go undiagnosed because there families lack the expenses needed to pay for Autism screening and diagnosing. Therefore, the development of a potential inexpensive, but accurate way to detect Autism in children is necessary for low-income families. With all the technological advances in Artificial Intelligence today, deep learning can be used to develop an effective method to detect Autism in children. This project utilizes a Convolutional Neural Network classifier to explore the possibility of using a facial image analysis to detect Autism in children. The facial images of Autistic and non-autistic male and female children will be used in this project.

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** Autism Spectrum Disorder, Detection, Artificial Intelligence, Deep Learning, Convolutional Neural Network. 

## 1. Introduction

Autism Spectrum Disorder (ASD) is a broad range of lifelong developmental and neurological disorders that usually appear during early childhood. Autism affects the brain and can cause challenges with speech and nonverbal communication, repetitive behaviors, and social skills. Autism Spectrum Disorder can occur in all socioeconomic, ethnic, and racial groups, and can usually be detected and diagnosed from the age of three years old and up. As of June 2021, the World Health Organization has estimated that one in 160 children have an Autism Spectrum Disorder worldwide[^1]. Early detection of Autism, along with treatment, is crucial to minimize some of the difficulties and symptoms that people with Autism face[^2]. Symptoms of Autism Spectrum Disorder are normally identified based on psychological criteria[^3]. Specialists use techniques such as behaivoral observation reports, questionaires, and a review of the child's cognitive ability to detect and diagose Autism in children. 

Many researchers believe that there is a correlation between facial morphology and Autism Spectrum Disorder, and that people with Autism have distinct facial features that can be used to detect their Autism Spectrum Disorder[^4]. Human faces encode important markers that can be used to detect Autism Spectrum Disorder by analyzing facial features, eye contact,facial movements, and more[^5]. Scientists found that children diagnosed with Autism share common facial feature distinctions from children who are not diagnosed with Autism[^6]. Some of these facial features are wide-set eyes, short middle region of the face, and a broad upper face. Figure 1 provides an example of the facial feature differences between a child with Autism and a child without.

![Autistic and Non-Autistic Child](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/Autistic%20compared%20with%20Non-Autistic%20(4).png)

**Figure 1:** Image of Child with Autism (left) and Child with no Autism (right)[^7].

Due to the distinct features of Autistic individuals, we believe that it is necessary to explore the possiblities of using a facial analysis to detect Autism in children,  using Artificial Intelligence (AI). Many researchers have attempted to explore the possibility of using various novel algorithms to detect and diagnose children, adolescents, and adults with Autism[^2]. Previous research has been done to determine if Autism Spectrum Disorder can be detected in children by analyzing a facial image[^7]. The author of this research collected approximately 1500 facial images of children with Autism from websites and Facebook pages associated with Autism. The facial images of non-autistic children were randomly downloaded from online and cropped.The author aimed to provide a first level screening for autism diagnosis, whereby parents could submit an image of their child and in return recieve a probability of the potential of Autism, without cost. 

To contribute to this previous research[^7], this project will propose a model that can be used to detect the presence of Autism in children based on a facial image analysis. 
A deep learning algorithm will be used to develop an inexpensive, accurate, and effective method to detect Autism in children. This project implements and utilizes a Convolutional Neural Network (CNN) classifier to explore the possibility of using a facial image analysis to detect Autism in children, with an accuracy of 95% or higher. Most of the coding used for this CNN model was obtained from the Kaggle dataset and was done by Fran Valuch[^8]. We made changes to some parts of this code, which will be discussed further in this project. The goal of this project is not to diagnose Autism, but to explore the possibility of detecting Autism at its early stage, using a facial image analysis. 

## 2. Related Work

Previous work exists on the use of artificial intelligence to detect Autism in children using a facial image. Most of this previous work used the Autism kaggle dataset[^7], which was also used for this project. One study utilized MobileNet followed by two dense layers in order to perform deep learning on the dataset[^6]. MobileNet was used because of its ability to compute outputs much faster, as it can reduce both computation and model size. The first layer was dedicated to distribution, and allowed customisation of weights to input into the second dense layer. The second dense layer allowed for classification. The architecture of this algorithm is shown below in Figure 2.

![Algorithm Architecture using MobileNet](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/2021-07-29.png)

**Figure 2:** Algorithm Architecture using MobileNet[^6].

Training of this model completed after fifteen epochs, which resulted in a test accuracy of 94.64%. In this project we will also utilize a classic Convolutional Neural Network model. This will be done in hopes of obtaining a test accuracy of 95% or higher.

## 3. Dataset

The dataset used for this project was obtained from Kaggle[^7]. This dataset contained approximately 1500 facial images of children with Autism that were obtained from websites and Facebook pages associated with Autism. The facial images of non-autistic children were randomly downloaded from online. The pictures obtained were not of the best quality or consistency with respect to the facial alignment. Therefore, the author developed a python program to automatically crop the images to include only the extent possible for a facial image. These images consist of male and female children that are of different races and range from around ages two to fourteen. 

This project uses version 12 of this dataset, which is the latest version. The dataset consists of three directories labled test, train, and valid, along with a CSV file. The training set is labeled as train, and consists of 'Autistic' and 'Non-Autistic' subdirectories. These subdirectories contain 1269 images of autistic and 1269 images of non-autistic children respectively. The validation set located in the valid directory are separated into 'Autistic' and 'Non-autistic' subdirectories. These subdirectories also contain 100 images of autistic and 100 images of non-autistic children respectively. The testing set located in the test directory is divided into 100 images of autistic children and 100 images of non-autistic children. All of the images provided in this dataset are in 224 X 224 X 3, jpg format. Table 1 provides a summary of the content in the dataset.

**Table 1:** Summary Table of Dataset.

![Summary Table of the Kaggle Dataset](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/DATASET%20BREAKDOWN.png)

## 4. Proposed Methodology

Convolutional Neural Network (CNN)

This project utilizes a Convolution Neural Network (CNN) to develop a program that can be used to detect the presence of Autism in children from a facial image analysis. If successful this program can be used an inexpensive method to detect Autism in children at its early stages. We believed that a CNN model would be the best way create this program because of its little dependence on preprocessing data. A Convolutional Neural Network was also used becuase of its ability to take in an image and assign importance to, and identify diferent objects within the image. CNN also has very high accuracy when dealing with image recognition. The dataset used contains 1269 training images that were used to train this Convolution Neural Network model. The architecture of this model can be seen in Figure 3.

![CNN Architecture](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/CNN%20Architecture.png)

**Figure 3:** Architecture of utilized Convolutional Neural Network Model.

## 5. Results

The results of this project is estimated by affectability and accuracy by utilizing the Confusion Matrix CNN. The results also rely on how correct and precise the model was trained. This model was created to explore the possibility of detecting Autism in children at its early stage, using a facial image analysis. A deep learning algorithm was used to develop this inexpensive, but accurate method to detect Autism in children. A Convolutional Neural Network (CNN) classifier was used to create this model, to recieve an accuracy of 95% or higher. For this CNN model we utilized max pooling and Rectified Linear Unit (ReLU), with two epochs. This resulted in an accuracy of 71%. These results can be seen below in Figure 4. Figure 5 displays some of the images that were classified and labeled correctly (right) and the others that were labeled incorrectly (left).

![Results after Execution](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/Training%20and%20Validation%20Loss%20and%20Accuracy%20(3).png)

**Figure 4:** Results after Execution.

validation loss: 57% - validation accuracy: 68% - training loss: 55% - training accuracy: 71%

![Correct and Incorrect Labels](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/Labels.png)

**Figure 5:** Correct Labels and Incorrect Labels.

## 6. Benchmark

![Confusion Matrix CNN](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/Confusion%20Matrix%20CNN.png)

**Figure 6:** Confusion Matrix CNN.

- [ ] Add info about CNN confusion matrix.
- [ ] Add next Benchmark
 
## 7. Conclusions and Future Work

Autism Spectrum Disorder is a broad range of lifelong developmental and neurological disorders that is considered one of the most growing disorders in children. The World Health Organization has estimated that one in 160 children have an Autism Spectrum Disorder worldwide[^1]. Techniques that are used by specialists to detect autism can be time consuming and inconvenient for some families. Considering these factors, finding effective and essential ways to detect Autism in children is a neccesity. The aim of this project was to create a model that would analyze facial images of children, and in return determine if the child is Autistic or not. This was done in hopes of receiving 95% accuracy or higher. After executing the model we received an accuracy of 71%. 

As shown in the results section above, some of the pictures that were initially labeled as Autistic, were labeled incorrectly after running the model. This low accuracy rate could be improved if the CNN model is combined with other algorithms such as transfer learning and VGG-19. This low accuracy could also be improved by using a dataset that includes a wider variety and larger amount of images. We could also ensure that images in the dataset includes children that are of a wider age range. These improvements could possibly increase our chances of obtaining an accuracy of 95% or higher. When this model is improved and an accuracy of atleast 95% is achieved, furture work can be done to create a model that can be used for Autistic individuals outside of the dataset age range (2 - 14 years old).

## 8. Acknowledgments

The author of this project would like to express a vote of thanks to Yohn Jairo, Carlos Theran, and Dr. Gregor von Laszewski for their encouragement and guidance throughout this project. A special vote of thanks also goes to Florida A&M University for funding this wonderful research program. The completion of this project could not have been possible without their support.

## 9. References

[^1]: World Health Organization. 2021. Autism spectrum disorders, [Online resource] <https://www.who.int/news-room/fact-sheets/detail/autism-spectrum-disorders>

[^2]: Raj, S., and Masood, S., 2020. Analysis and Detection of Autism Spectrum Disorder Using Machine Learning Techniques, [Online resource <https://reader.elsevier.com/reader/sd/pii/S1877050920308656?token=D9747D2397E831563D1F58D80697D9016C30AAC6074638AA926D06E86426CE4CBF7932313AD5C3504440AFE0112F3868&originRegion=us-east-1&originCreation=20210704171932>

[^3]: Khodatars, M., Shoeibi, A., Ghassemi, N., Jafari, M., Khadem, A., Sadeghi, D., Moridian, P., Hussain, S., Alizadehsani, R., Zare, A., Khosravi, A., Nahavandi, S., Acharya, U. R., and Berk, M., 2020. Deep Learning for Neuroimaging-based Diagnosis and Rehabilitation of Autism Spectrum Disorder: A Review. [Online resource] <https://arxiv.org/pdf/2007.01285.pdf>

[^4]: Musser, M., 2020. Detecting Autism Spectrum Disorder in Children using Computer Vision, Adapting facial recognition models to detect Autism Spectrum Disorder. [Online resource] <https://towardsdatascience.com/detecting-autism-spectrum-disorder-in-children-with-computer-vision-8abd7fc9b40a>

[^5]: Akter, T., Ali, M. H., Khan, I., Satu, S., Uddin, Jamal., Alyami, S. A., Ali, S., Azad, A., and Moni, M. A., 2021. Improved Transfer-Learning-Based Facial Recognition Framework to Detect Autistic Children at an Early Stage. [Online resource] <https://www.mdpi.com/2076-3425/11/6/734>

[^6]: Beary, M., Hadsell, A., Messersmith, R., Hosseini, M., 2020. Diagnosis of Autism in Children using Facial Analysis and Deep Learning. [Online resource] <https://arxiv.org/ftp/arxiv/papers/2008/2008.02890.pdf>

[^7]: Piosenka, G., 2020. Detect Autism from a facial image. [Online resource] <https://www.kaggle.com/gpiosenka/autistic-children-data-set-traintestvalidate?select=autism.csv>

[^8]: Valuch, F., 2021. Easy Autism Detection with TF.[Online resource] <https://www.kaggle.com/franvaluch/easy-autism-detection-with-tf/comments>
