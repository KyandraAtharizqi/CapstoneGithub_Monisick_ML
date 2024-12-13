
# Monisick Machine Learning Path

This is the GitHub Repository for Machine Learning Team of the Monisick Capstone Project.




## Members
- M318B4KY3583 - Rafi Kyandra Atharizqi - Universitas Sultan Ageng Tirtayasa
- M318B4KX4474 - Widi Tri Nurhasanah - Universitas Sultan Ageng Tirtayasa
- M318B4KX1779 - Hikayati Oktaviyani - Universitas Sultan Ageng Tirtayasa
## Idea
During medication period, Medication Adherence is an issue that is sometimes faced by a number of patients.  The issues can stems from forgetfulness to personal belief. Some research also suggest the factor of social support.  Moreover, lack of oversight for patient nutritional need, or daily documentation of their condition can be a hurdle for healthcare professionals to assess the effectiveness of medication period.

Monisick is an application that is used to monitor sick people, by reminding them to take their medicine, predicting the nutrient of their meal, and a way to document their condition daily. The app can be used by the patient or caregiver.  It is designed to support patients or their caregivers in maintaining health during a medication period. Caregivers can be a form of social support, especially for elderly or children. We hope by providing this tool, it will strengthen the bond between them, thus supporting the patient during the medication period.

We realize that the information needs to be reviewed by a professional to give an insight of the medication period effectiveness. The information collected in the application aims to be useful for them to do analysis of the patient condition/recovery process out of this.

Monisick will use a Machine Learning model for Nutrition Prediction feature, where user can take an image of their food and the model will predict the following: (in gram)

- Weights
- Carbohydrates
- Protein
- Fat


## Dataset

We use a sample of **Nutrition5k** dataset that is available in Kaggle to train the model
[Kaggle](https://www.kaggle.com/datasets/zygmuntyt/nutrition5k-dataset-side-angle-images)




The original source of **Nutrition5k** can be located here
[GitHub](https://github.com/google-research-datasets/Nutrition5k)

- 4793 Unique Dishes
- Unique images for each dish
- Total Weight, Carbohydrates, Fat, and Protein per gram data for each dish
## Data Preprocessing
We rearrange some columns of the CSV for convenience. Then we removed dishes that has deprecated or invalid datas. After that, we augment images on each dish, to make sure that every dish has at least 10 images. Lastly, we splitted the dish into Training, Validation, and Test set.
## Technology
We build the model using the Tensorflow and Keras libraries.

We use a non-linear regression method for the model, it leverages ResNet50 as base for transfer learning to our dataset. We use ResNet50 for it's performance being better than other model like InceptionV3 or MobileNet. After that, we add additional layers such as Dense Layers with Relu Activation and L2 Regularizers, Batch Normalization Layers and Dropout layers. 


## The Model
Due to GitHub limitation, we uploaded the model [Here](https://drive.google.com/file/d/12s3jkJhuIVmiFc4SDDjXBvzoPIkr_oO7/view?usp=drive_link)
## Machine Learning API Code
This is a repository for the inference code, we build this in close collaboration with the Cloud Computing team

[ML API](https://www.kaggle.com/datasets/zygmuntyt/nutrition5k-dataset-side-angle-images)
## Related Monisick Repositories
Here are the related repositories for other paths of our Project

- [Cloud Computing](https://github.com/KyandraAtharizqi/CapstoneGithub_Monisick_ML)
- [Mobile Development](https://github.com/HassZen/Monisick)