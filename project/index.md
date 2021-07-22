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

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** Autism Spectrum Disorder, Detection, Artificial Intelligence, Deep Learning, Convolutional Neural Network, Computer Vision. 

## 1. Introduction

Autism Spectrum Disorder (ASD) is a broad range of lifelong developmental and neurological disorders that usually appear during early childhood. Autism affects the brain and can cause challenges with speech and nonverbal communication, repetitive behaviors, and social skills. Autism Spectrum Disorder can occur in all socioeconomic, ethnic, and racial groups. This neurological disorder can usually be detected and diagnosed from the age of three years old and up. As of June 2021, the World Health Organization has estimated that one in 160 children have an Autism Spectrum Disorder worldwide[^1]. Early detection and diagnosis of Autism, along with treatment, is crucial to minimize some of the difficulties and symptoms that people with Autism face[^2]. Symptoms of Autism Spectrum Disorder are normally identified based on psychological criteria[^3]. 

Techniques used in Machine Learning help research dimensions of medical diagnosis. Many researchers have attempted to explore the possibility of using various novel algorithms to detect and diagnose children, adolescents, and adults with Autism[^2]. Researchers believe that there is a correlation between facial morphology and Autism Spectrum Disorder, and that people with Autism have distinct facial features that can be used to detect their Autism Spectrum Disorder[^4]. Human faces encode important markers that can be used to detect Autism Spectrum Disorder by analyzing facial features, eye contact,facial movements, and more[^5]. Therefore, machine learning can be used to develop a program where facial images can be analyzed to detect Autism in children.

Previous research has been done to determine if Autism Spectrum Disorder can be detected in children by analyzing a facial image[^6]. The author of this research collected approximately 1500 facial images of children with Autism from websites and Facebook pages associated with Autism. The pictures obtained were not of the best quality or consistency with respect to the facial alignment. Therefore, the author developed a python program to automatically crop the images to include only the extent possible for a facial image. The facial images of non-autistic children were randomly downloaded from online and cropped. The author set about creating a CNN classifier on this data set, and had already developed a General Purpose CNN with multiple model options. The goal was to achieve 95% accuracy with a low false alarm rate.

This previous research aimed to create a no cost means to provide a first level screening for autism diagnosis, whereby parents could submit an image of their child and in return recieve a probability of the potential of Autism. To contribute to this previous research, this project will analyze facial images of Autistic and non-autistic male and female children using Artificial Intelligence. The goal of this project is not to diagnose Autism, but to explore the possibility of detecting Autism in children using a facial image. A deep learning algorithm will be used to develop an inexpensive, accurate, and effective method to detect Autism in children. This project utilizes a Convolutional Neural Network classifier to explore the possibility of using a facial image analysis to detect Autism in children. 

- [ ] Talk about accuracy predictions and goals.
- [ ] ADD PARAGRAPH ABOUT ETHICS IN AUTISM.

## 2. Related Work

- [ ] Talk about previous work that has been done.
- [ ] Talk about algorithms used and accuracy received.
- [ ] Talk about how this will help with my work.
- [ ] Add Images

## 3. Dataset

The dataset used for this project was obtained from Kaggle[^7]. This dataset was chosen because it provides a variety of images of Autistic and Non-autistic children that were already cropped to show only the child's face. It includes sufficient information about the correlation between facial morphology and Autism. It also includes feedback and numerous codes done by other contributers. The author of this dataset collected approximately 1500 facial images of children with Autism from websites and Facebook pages associated with Autism. He developed a python program to automatically crop the images to include only the extent possible for a facial image. The facial images of non-autistic children were randomly downloaded from online and cropped. This project uses version 12 of this dataset, which is the latest version. The dataset consists of three directories labled test, train, and valid, along with a CSV file. The training set is labeled as train, and consists of 'Autistic' and 'Non-Autistic' subdirectories. These subdirectories contain 1269 images of autistic and 1269 images of non-autistic children respectively. The validation set located in the valid directory are separated into 'Autistic' and 'Non-autistic' subdirectories. These subdirectories also contain 100 images of autistic and 100 images of non-autistic children respectively. The testing set located in the test directory is divided into 100 images of autistic children and 100 images of non-autistic children. All of the images provided in this dataset are in 224 X 224 X 3, jpg format. 

**Figure 1:** Child with Autism[^7].

![Autistic Child](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/Autism(1).jpg)

**Figure 2:** Child without Autism[^7].

![Non-autistic Child](https://raw.githubusercontent.com/cybertraining-dsc/su21-reu-378/main/project/images/No%20Autism.jpg)

- [ ] Be more specific on the children used in the dataset. For example, talk about the age range, race, and gender ratios.

## 4. Architecture
****Convolutional Neural Network

- [ ] Add brief description about CNN.
- [ ] Tell how it will be used for this project.
- [ ] Add an image.

## 5. Implementation

## 6. Results and Discussion

- [ ] Talk about the results obtained.
- [ ] Include Images.

## 6. Benchmark

Your project must include a benchmark. The easiest is to use cloudmesh-common [^2]
 
## 7. Conclusion

A convincing but not fake conclusion should summarize what the conclusion of the project is.
- [ ] State if goal was met, then explain.
- [ ] Talk about problems experienced/limitations.

## 8. Future Work

Talk about what work will be done in the future.
- [ ] Work on a model that can be used for children outside of the dataset age range, i.e teenagers.
- [ ] Work on model that trains data for children of all colors, i.e people of color.
- [ ] Continue working on model to achieve accuracy above 95%.

## 9. Acknowledgments

The author of this project would like to express a vote of thanks to Yohn Jairo, Carlos Theran, and Dr. Gregor von Laszewski for their encouragement and guidance throughout this project. A special vote of thanks also goes to Florida A&M University for funding this wonderful research program. The completion of this project could not have been possible without their support.

## 10. References

[^1]: World Health Organization. 2021. Autism spectrum disorders, [Online resource] <https://www.who.int/news-room/fact-sheets/detail/autism-spectrum-disorders>

[^2]: Raj, S., and Masood, S., 2020. Analysis and Detection of Autism Spectrum Disorder Using Machine Learning Techniques, [Online resource <https://reader.elsevier.com/reader/sd/pii/S1877050920308656?token=D9747D2397E831563D1F58D80697D9016C30AAC6074638AA926D06E86426CE4CBF7932313AD5C3504440AFE0112F3868&originRegion=us-east-1&originCreation=20210704171932>

[^3]: Khodatars, M., Shoeibi, A., Ghassemi, N., Jafari, M., Khadem, A., Sadeghi, D., Moridian, P., Hussain, S., Alizadehsani, R., Zare, A., Khosravi, A., Nahavandi, S., Acharya, U. R., and Berk, M., 2020. Deep Learning for Neuroimaging-based Diagnosis and Rehabilitation of Autism Spectrum Disorder: A Review. [Online resource] <https://arxiv.org/pdf/2007.01285.pdf>

[^4]: Musser, M., 2020. Detecting Autism Spectrum Disorder in Children using Computer Vision, Adapting facial recognition models to detect Autism Spectrum Disorder. [Online resource] <https://towardsdatascience.com/detecting-autism-spectrum-disorder-in-children-with-computer-vision-8abd7fc9b40a>

[^5]: Akter, T., Ali, M. H., Khan, I., Satu, S., Uddin, Jamal., Alyami, S. A., Ali, S., Azad, A., and Moni, M. A., 2021. Improved Transfer-Learning-Based Facial Recognition Framework to Detect Autistic Children at an Early Stage. [Online resource] <https://www.mdpi.com/2076-3425/11/6/734>

[^6]: Piosenka, G., 2020. Detect Autism from a facial image. <https://www.kaggle.com/gpiosenka/autistic-children-data-set-traintestvalidate?select=autism.csv>
