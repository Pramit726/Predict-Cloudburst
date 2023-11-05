# Advancing Cloudburst Prediction with Mixed-Input Deep Learning: Combining CNN and Feed-Forward Neural Networks
Train a multi-modal deep learning scheme (combining CNN and FNN) to predict cloudburst events using INSAT3D images and ERA5 hourly temperature and precipitation data. 

## Input data
- Satellite images from INSAT3D collected from Meteorological and Oceanographic Satellite Data Archival Centre(https://mosdac.gov.in/) [4]during the occurrence of cloud bursts, as well as 6 hours prior and 6 hours after the cloudburst. Images of random noncloudburst events  
- satellite images were labeled into 4 categories: 'cloudburst,' 'precloudburst', 'postcloudburst', and 'no cloudburst  
- ERA5 Climate reanalysis data (hourly temperature and precipitation) from CDS store (https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=form) converted into .csv format  

## Functionality
- Preprocess data: the script preprocess corresponding spatial satellite images and tabular climate data from ERA5 and merge them  
- Splitting into train, validation, and test set : the processed data is shuffled and split into train, validation, and test dataset  
- Model architecture :  a model architecture is defined by combining a CNN (MobileNetV2) and FNN  
- Model optimization: the defined model is optimized using ADAM algorithm in 10 epochs and model loss and accuracy were collected for each epoch  
- Visualization : model loss and accuracy are plotted to visualize if model accuracy is getting better with each epoch  
- Model testing : the best performing trained model is tested on the test dataset and model accuracy and loss on test dataset are printed  

## Future scope
- The trained multi-model DL scheme can be fed with real-time satellite images and weather data to predict cloudburst risk.
- If a cloudburst risk is detected, automatic notifications can be sent to concerned authorities for disaster readiness and evacuation planning.  

## Dependencies
- Pandas  
- Numpy  
- cv2  
- Matplotlib  
- TensorFlow 

## Contributor
- Pramit De (email: pramitde726@gmail.com/pramit.de.cse.2021@tint.edu.in) (Department of CSE, Techno International Newtown, West Bengal, India)   
   


