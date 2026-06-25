<img width="3102" height="1752" alt="Cow Data Sorting Process - visual selection (2)" src="https://github.com/user-attachments/assets/660aa1ff-2205-4025-bb4e-a8f8301d4e3a" />
<img width="2624" height="894" alt="Cow Data Sorting Process - visual selection (3)" src="https://github.com/user-attachments/assets/26345264-c360-4304-a3fb-8564ca84e9e5" />

Lets start!

There were 18,000+ cow videos.  

First I decided to separate them into videos where only one cow was present and videos where more than one cow was present.

c01 was wrote for this purpose, it uses code from 'Study05.2.1_PyTorchVideoDataLoader_Swin3D_ToSaveTrainedModel_MiscIncluded' in Video_Classification_Swin3D Repo.  
c01_Cow_Swin3D_VideoClassifier_SingularOrPlural_ModelTrain

But swin3D was too slow so switched to x3d, c02 was wrote for this, it uses code from 'Study07.1_PyTorchVideoDataLoader_x3d_ToSaveTrainedModel_MiscIncluded' in Video_Classification_Swin3D Repo.  
c02.1_Cow_x3d_VideoClassifier_SingularOrPlural_ModelTrain  
c02.2_Cow_x3d_VideoClassifier_SingularOrPlural_CallingAndUsingTrainedModel  
c02.3_Cow_x3d_VideoClassifier_SingularOrPlural_CallingAndUsingTrainedModel_SortingAllVideos

Now that most 'Singular cow' in frame videos were extracted,  
They were fed as input for the eat, rest or walk/stand sorter c03.  
c03.1_Cow_x3d_VideoClassifier_EatRestWalk_ModelTrain  
c03.2_Cow_x3d_VideoClassifier_EatRestWalk_CallingAndUsingTrainedModel  
c03.3_Cow_x3d_VideoClassifier_EatRestWalk_CallingAndUsingTrainedModel_SortingAllVideos  

The sorted videos goes to different bins:
Predicted_cow_eat  
Predicted_cow_rest  
Predicted_cow_walk_stand  
Predicted_Miscellaneous  




