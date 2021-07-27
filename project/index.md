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

{{% pageinfo %}}

## Abstract

Autism affects 1 in every 160 children worlwide. Early detection and diagnosis of Autism, along with treatment, is needed to minimize some of the difficulties that people with Autism encounter. Autism is usually diagnosed by a specialist through various Autism screening methnods. This can be an expensive and complex process. Many children that display signs of Autism go undiagnosed because there families lack the expenses needed to pay for Autism screening and diagnosing. Therefore, the development of a potential inexpensive, but accurate way to detect Autism in children is necessary for low-income families. With all the technological advances in Artificial Intelligence today, deep learning can be used to develop an effective method to detect Autism in children. This project utilizes a Convolutional Neural Network classifier to explore the possibility of using a facial image analysis to detect Autism in children. The facial images of Autistic and non-autistic male and female children will be used in this project.

- [ ] Add a bit more

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** Autism Spectrum Disorder, Detection, Artificial Intelligence, Deep Learning, Convolutional Neural Network, Computer Vision. 

## 1. Introduction

Autism Spectrum Disorder (ASD) is a broad range of lifelong developmental and neurological disorders that usually appear during early childhood. Autism affects the brain and can cause challenges with speech and nonverbal communication, repetitive behaviors, and social skills. Autism Spectrum Disorder can occur in all socioeconomic, ethnic, and racial groups, and can usually be detected and diagnosed from the age of three years old and up. As of June 2021, the World Health Organization has estimated that one in 160 children have an Autism Spectrum Disorder worldwide[^1]. Early detection of Autism, along with treatment, is crucial to minimize some of the difficulties and symptoms that people with Autism face[^2]. Symptoms of Autism Spectrum Disorder are normally identified based on psychological criteria[^3]. Specialists use techniques such as behaivoral observation reports, questionaires, and a review of the child's cognitive ability to detect and diagose Autism in children. 

Many researchers believe that there is a correlation between facial morphology and Autism Spectrum Disorder, and that people with Autism have distinct facial features that can be used to detect their Autism Spectrum Disorder[^4]. Human faces encode important markers that can be used to detect Autism Spectrum Disorder by analyzing facial features, eye contact,facial movements, and more[^5]. Scientists found that children diagnosed with Autism share common facial feature distinctions from children who are not diagnosed with Autism[^6]. Some of these facial features are wide-set eyes, short middle region of the face, and a broad upper face. Image one provides an example of the facial feature differences between a child with Autism and a child without.

Due to the distinct features of Autistic individuals, we believe that it is necessary to explore the possiblities of using a facial analysis to detect Autism in children,  using Artificial Intelligence (AI). Many researchers have attempted to explore the possibility of using various novel algorithms to detect and diagnose children, adolescents, and adults with Autism[^2]. Previous research has been done to determine if Autism Spectrum Disorder can be detected in children by analyzing a facial image[^7]. The author of this research collected approximately 1500 facial images of children with Autism from websites and Facebook pages associated with Autism. The facial images of non-autistic children were randomly downloaded from online and cropped.The author aimed to provide a first level screening for autism diagnosis, whereby parents could submit an image of their child and in return recieve a probability of the potential of Autism, without cost. 

To contribute to this previous research[^7], this project will propose a model that can be used to detect the presence of Autism in children based on a facial image analysis. 
A deep learning algorithm will be used to develop an inexpensive, accurate, and effective method to detect Autism in children. This project implements and utilizes a Convolutional Neural Network (CNN) classifier to explore the possibility of using a facial image analysis to detect Autism in children. Most of the coding used for this CNN model was obtained from the Kaggle dataset and was done by Fran Valuch[^8]. We made changes to some parts of this code, which will be discussed further in this project. The goal of this project is not to diagnose Autism, but to explore the possibility of detecting Autism at its early stage, using a facial image analysis. 

## 2. Related Work

- [ ] Talk about previous work that has been done.
- [ ] Talk about algorithms used and accuracy received.
- [ ] Talk about how this will help with my work.
- [ ] Add Images.
- [ ] State how mine will be done differently.

## 3. Dataset

The dataset used for this project was obtained from Kaggle[^7]. This dataset contained approximately 1500 facial images of children with Autism that were obtained from websites and Facebook pages associated with Autism. The facial images of non-autistic children were randomly downloaded from online. The pictures obtained were not of the best quality or consistency with respect to the facial alignment. Therefore, the author developed a python program to automatically crop the images to include only the extent possible for a facial image. These images consist of male and female children that are of different races and range from around ages two to fourteen. 

This project uses version 12 of this dataset, which is the latest version. The dataset consists of three directories labled test, train, and valid, along with a CSV file. The training set is labeled as train, and consists of 'Autistic' and 'Non-Autistic' subdirectories. These subdirectories contain 1269 images of autistic and 1269 images of non-autistic children respectively. The validation set located in the valid directory are separated into 'Autistic' and 'Non-autistic' subdirectories. These subdirectories also contain 100 images of autistic and 100 images of non-autistic children respectively. The testing set located in the test directory is divided into 100 images of autistic children and 100 images of non-autistic children. All of the images provided in this dataset are in 224 X 224 X 3, jpg format. 

**Image 1:** Image of Child with Autism (left) and Child with no Autism (right)[^7].

![Autistic and Non-Autistic Child](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/Autistic%20compared%20with%20Non-Autistic%20(4).png)

## 4. Architecture

Convolutional Neural Network

## 5. Implementation

## 6. Results and Discussion

- [ ] Talk about the results obtained.
- [ ] Include Images.

## 7. Benchmark

Your project must include a benchmark. The easiest is to use cloudmesh-common [^2]
 
## 8. Conclusion

A convincing but not fake conclusion should summarize what the conclusion of the project is.
- [ ] State if goal was met, then explain.
- [ ] Talk about problems experienced/limitations.

## 9. Future Work

Talk about what work will be done in the future.
- [ ] Work on a model that can be used for children outside of the dataset age range, i.e teenagers.
- [ ] Work on model that trains data for children of all colors, i.e people of color.
- [ ] Continue working on model to achieve accuracy above 95%.

## 10. Acknowledgments

The author of this project would like to express a vote of thanks to Yohn Jairo, Carlos Theran, and Dr. Gregor von Laszewski for their encouragement and guidance throughout this project. A special vote of thanks also goes to Florida A&M University for funding this wonderful research program. The completion of this project could not have been possible without their support.

## 11. References

[^1]: World Health Organization. 2021. Autism spectrum disorders, [Online resource] <https://www.who.int/news-room/fact-sheets/detail/autism-spectrum-disorders>

[^2]: Raj, S., and Masood, S., 2020. Analysis and Detection of Autism Spectrum Disorder Using Machine Learning Techniques, [Online resource <https://reader.elsevier.com/reader/sd/pii/S1877050920308656?token=D9747D2397E831563D1F58D80697D9016C30AAC6074638AA926D06E86426CE4CBF7932313AD5C3504440AFE0112F3868&originRegion=us-east-1&originCreation=20210704171932>

[^3]: Khodatars, M., Shoeibi, A., Ghassemi, N., Jafari, M., Khadem, A., Sadeghi, D., Moridian, P., Hussain, S., Alizadehsani, R., Zare, A., Khosravi, A., Nahavandi, S., Acharya, U. R., and Berk, M., 2020. Deep Learning for Neuroimaging-based Diagnosis and Rehabilitation of Autism Spectrum Disorder: A Review. [Online resource] <https://arxiv.org/pdf/2007.01285.pdf>

[^4]: Musser, M., 2020. Detecting Autism Spectrum Disorder in Children using Computer Vision, Adapting facial recognition models to detect Autism Spectrum Disorder. [Online resource] <https://towardsdatascience.com/detecting-autism-spectrum-disorder-in-children-with-computer-vision-8abd7fc9b40a>

[^5]: Akter, T., Ali, M. H., Khan, I., Satu, S., Uddin, Jamal., Alyami, S. A., Ali, S., Azad, A., and Moni, M. A., 2021. Improved Transfer-Learning-Based Facial Recognition Framework to Detect Autistic Children at an Early Stage. [Online resource] <https://www.mdpi.com/2076-3425/11/6/734>

[^6]: Beary, M., Hadsell, A., Messersmith, R., Hosseini, M., 2020. Diagnosis of Autism in Children using Facial Analysis and Deep Learning. [Online resource] <https://arxiv.org/ftp/arxiv/papers/2008/2008.02890.pdf>

[^7]: Piosenka, G., 2020. Detect Autism from a facial image. [Online resource] <https://www.kaggle.com/gpiosenka/autistic-children-data-set-traintestvalidate?select=autism.csv>

[^8]: Valuch, F., 2021. Easy Autism Detection with TF.[Online resource] <https://www.kaggle.com/franvaluch/easy-autism-detection-with-tf/comments>
