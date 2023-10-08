# Iitiansindenorth
GeoAI Reimagined challenge in Nasa Space Apps
Team Name - IITians_In_De_North  
Problem Statement - GeoAI Reimagined: Transformative and Diverse Earth Science Applications Using Foundation Models
Team Leader Email - hryadyanshsaraswat@gmail.com

**A Brief of the Prototype:**
The problem statement wanted us to develop AI models which can help researchers geospatial analytics tasks. There is an acute shortage of properly labelled satelite data as most of the time this data is manually labelled. As a result, the AI models which have to perform geospatial analytics tasks need to either levrage existing pre trained foundation model or to make good use of the existing labelled satelite data. These AI models will not only help in literal tasks like land classification, change detection, building detection, objection detection, calamity detection, crop classifiation and/or biomass estimation. But these models when used together can fulfuill various different kinds of tasks and infer infomation, predict state of remote areas where else it would have been very difficult to do so. (For example:- Let a place be a residential area, with many houses. There used to be apmle of light in the night photos of that region due to the houses present there. But after some time it was detected that slowly slowly light from each house started to reduce. This could help us infer that people may be leaving that place. Or, it may also tell us that there can be a disease spread. The confidence interval of the notion of disease spread could be found out by calcuating the biomass in the nearby areas. If the biomass in the nearby areas may also be decreasing. It may further boost the notion that there is a diease spread). These examples will become more clear as we proceed.

The models created by us in the protoype are :-
**1. Land Classification:-** Trained on the eurosat data which is labelled by euro atlas, a very information constrained data. The model classifies the land into different segments, while also efficiently using the data. The model is able to efficiently use the 64x64 data becuase it levrages the foundation model wide_resnet50_2 via transfer learning.
Here are the accuracy parameters of the model, confusion matrix and a sample output:-
LR = 0.0001, Batch_size = 64, Optimiser = RMSprop, Train Loss = 0.5707, Train Accuracy = 0.8189, Val Loss = 0.5327, Val Acc = 0.829, 
Val Precision = 0.8276, Val F1 = 0.827, Val AUC = 0.9049

Confusion Matrix:-
https://drive.google.com/file/d/1ZAhnTckLOYHeLLR35ujIaKjLvcP2xZX-/view?usp=sharing

The model is self trained by us with 10 epochs.





**UML Digrams:**
To do the extra and harmonic tasks which we wish to achieve, we have deployed the following pipeline :-
https://drive.google.com/file/d/1QF3N-0yhgliaecsc5R6C3f71Nhp8fHRp/view?usp=sharing

**Tech Stack:**
1. AI/ML
2. Deep Learning
3. Transformers (Models Fine Tuned from Prithvi 100M)
4. Transfer Learning and Fine Tuning (In all trained models except building classification)
5. PPrithvi 100 M foundation model
6. Wide_Resnet50_2 foundation model
7. CNN
8. Segmentation
9. Masking








