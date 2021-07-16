---
date: 2021-06-16
title: "Project: Detection of Autism Spectrum Disorder with a Facial Image using Artificial Intelligence"
linkTitle: Autism
tags: ["project", "reu","AI",Autism Spectrum Disorder"]
description: "Analyzing Facial Images to Detect Austism Spectrum Disorder using AI"
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

Autism affects 1 in every 160 children worlwide, early detection and diagnosis of Autism, along with treatment, is needed to minimize some of the difficulties that people with Autism encounter. Autism can sometimes be difficult to detect, especially if the individual is on the higher-functioning end of the spectrum. Machine Learning can develop an effective method to detect and diagnose people with Autism. Many researchers believe that there is a correlation between facial morphology and Autism Spectrum Disorder. This project explores the possibility of using a facial image analysis to detect Autism in children. The facial images of Autistic and non-autistic male and female children will be analyzed using Artificial Intelligence.

- [ ] ADD MORE INFO TO ABSTRACT.

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

**Keywords:** Autism Spectrum Disorder, Detect, Analysis, Image Data, Computer Vision. 

## 1. Introduction

Autism Spectrum Disorder (ASD) is a broad range of lifelong developmental and neurological disorders that usually appear during early childhood. Autism affects the brain and can cause challenges with speech and nonverbal communication, repetitive behaviors, and social skills. Autism Spectrum Disorder can occur in all socioeconomic, ethnic, and racial groups. This neurological disorder can usually be detected and diagnosed from the age of three years old and up. As of June 2021, the World Health Organization has estimated that one in 160 children have an Autism Spectrum Disorder worldwide[^1]. Early detection and diagnosis of Autism, along with treatment, is crucial to minimize some of the difficulties and symptoms that people with Autism face[^2]. Symptoms of Autism Spectrum Disorder are normally identified based on psychological criteria[^3]. 

Machine Learning is a branch of Artificial Intelligence that has the potential to substantially enhance the role of computational methods in neuroscience[^4].  Techniques used in Machine Learning help research dimensions of medical diagnosis, many researchers have attempted to explore the possibility of using various novel algorithms to detect and diagnose children, adolescents, and adults with Autism[^2]. Researchers believe that there is a correlation between facial morphology and Autism Spectrum Disorder. Many researchers believe that people with Autism have distinct facial features that can be used to detect their Autism Spectrum Disorder[^5]. Human faces encode important markers that can be used to detect Autism Spectrum Disorder by analyzing facial features, eye contact,facial movements, and more[^6]. 

Previous research has been done to determine if Autism Spectrum Disorder can be detected in children by analyzing a facial image[^7]. The author of this research collected about 1500 facial images of children with Autism from websites and Facebook pages associated with Autism. The pictures obtained were not of the best quality or consistency with respect to the facial alignment. Therefore, the author developed a python program to automatically crop the images to include only the extent possible for a facial image. The facial images of non-autistic children were randomly downloaded from online and cropped. The author set about creating a CNN classifier on this data set, and had already developed a General Purpose CNN with multiple model options. The model used was derived from transfer learning using MobileNet V1, and the best accuracy achieved was approximately 93% accuracy on the test set. The minimum goal was to achieve 95% accuracy with a low false alarm rate.

This previous research aimed to create a no cost means to provide a first level screening for autism diagnosis, whereby parents could submit an image of their child and in return recieve a returned probability of the potential of Autism. To contribute to this previous research, this project will analyze facial images of Autistic and non-autistic male and female children using Artificial Intelligence. The goal is to show how a facial image analysis could possibly be used to detect Autism Spectrum Disorder in children. 

## 2. Methodology

What will be done to carry out this project? what methodology they used ? 

* Convolutional Neural Network

## 3. Images

![Figure 1](https://github.com/cybertraining-dsc/fa20-523-314/raw/main/project/images/chart.png)

**Figure 1:** Images can be included in the report, but if they are copied you must cite them [^1].

## 4. Datasets

* <https://www.kaggle.com/gpiosenka/autistic-children-data-set-traintestvalidate?select=autism.csv>

The dataset used for this project is a CSV file that contains the filepaths, labels, and dataset relative to this study. It is provided to be used in two ways, which are both standard for machine learning tasks. For the first standard method, the data is divided into Training, Test, and Validation sets. The training set is labeled as train, and consists of 'Autistic' and 'Non-Autistic' subdirectories. The Autistic and Non-Autistic subdirectories consist of 1667 facial images of Autistic children and 1667 facial images of Non-Autistic children respectively, in 224 X 224 X 3, jpg format. The validation images located in the valid directory are separated into 50 images of autistic children and 50 images of non-autistic children in the same format as for the training set. The test data located in the test directory is divided into 100 images of autistic children and 100 images of non-autistic children. The second way the data is provided is in the consolidated directory. This directory also has the two sub directories of Autistic and Non_Autistic. It represents the consolidation of the files from the train, test and valid directories into a single set. 

- [ ] ADD PARAGRAPH ABOUT ETHICS IN AUTISM.
- [ ] FIX INFO IN DATA SET PARAGRAPH. (VERSION 12)

## 5. Benchmark

Your project must include a benchmark. The easiest is to use cloudmesh-common [^2]
 
## 6. Conclusion

A convincing but not fake conclusion should summarize what the conclusion of the project is.

## 7. Acknowledgments

The author of this project would like to express a vote of thanks to Yohn Jairo, Carlos Theran, and Dr. Gregor von Laszewski for their encouragement and guidance throughout this project. A special vote of thanks also goes to Florida A&M University for funding this wonderful research program. The completion of this project could not have been possible without their support.

## 8. References

[^1]: World Health Organization. 2021. Autism spectrum disorders, [Online resource] <https://www.who.int/news-room/fact-sheets/detail/autism-spectrum-disorders>

[^2]: Raj, S., and Masood, S., 2020. Analysis and Detection of Autism Spectrum Disorder Using Machine Learning Techniques, [Online resource <https://reader.elsevier.com/reader/sd/pii/S1877050920308656?token=D9747D2397E831563D1F58D80697D9016C30AAC6074638AA926D06E86426CE4CBF7932313AD5C3504440AFE0112F3868&originRegion=us-east-1&originCreation=20210704171932>

[^3]: Khodatars, M., Shoeibi, A., Ghassemi, N., Jafari, M., Khadem, A., Sadeghi, D., Moridian, P., Hussain, S., Alizadehsani, R., Zare, A., Khosravi, A., Nahavandi, S., Acharya, U. R., and Berk, M., 2020. Deep Learning for Neuroimaging-based Diagnosis and Rehabilitation of Autism Spectrum Disorder: A Review. [Online resource] <https://arxiv.org/pdf/2007.01285.pdf>

[^4]: Eslami, T., Almuqhim, F., Raiker, J. S., and Saeed, F., 2021. Machine Learning Methods for Diagnosing Autism Spectrum Disorder and Attention- Deficit/Hyperactivity Disorder Using Functional and Structural MRI: A Survey [Online resource] <https://www.frontiersin.org/articles/10.3389/fninf.2020.575999/full#B50>

[^5]: Musser, M., 2020. Detecting Autism Spectrum Disorder in Children using Computer Vision, Adapting facial recognition models to detect Autism Spectrum Disorder. [Online resource] <https://towardsdatascience.com/detecting-autism-spectrum-disorder-in-children-with-computer-vision-8abd7fc9b40a>

[^6]: Akter, T., Ali, M. H., Khan, I., Satu, S., Uddin, Jamal., Alyami, S. A., Ali, S., Azad, A., and Moni, M. A., 2021. Improved Transfer-Learning-Based Facial Recognition Framework to Detect Autistic Children at an Early Stage. [Online resource] <https://www.mdpi.com/2076-3425/11/6/734>

[^7]: Gerry, 2020. Detect Autism from a facial image. <https://www.kaggle.com/gpiosenka/autistic-children-data-set-traintestvalidate?select=autism.csv>
