# Laxya Agarwal-IITB-Assignment

For running RestAPI webapp 
simply do  https://laxyaattention.onrender.com 
# python app.py 
This project builds an Attention-OCR Model by generating synthetic data and training it on aocr.
Please check out my saved model it is givig 99% accuracy ,
File Structure:
./out  showing the model performance on test data <br />

./ loss graph showing the loss <br />

![loss graph ](https://github.com/laksh9950/Laxya_Agarwal-IITB-Assignment/blob/master/loss%20smooth.png)

./ test results on real world data <br />

![test results  ](https://github.com/laksh9950/Laxya_Agarwal-IITB-Assignment/blob/master/test%20results.PNG) <br />

./Background_Images_and_Fonts <br />
  Consists of different background images and font list which are necessary while implementing text-renderer
  
./attention-ocr-master  <br />
  It's a github repo by user "emedvedev" and can be located here : https://github.com/emedvedev/attention-ocr
  It's been modified according to the requirements and modifications are mentioned in the report as well as     instructions.txt
  
./checkpoints  <br />
  It has the generated checkpoints while training.
 
./datasets/synthetic   <br />
  It contains sample images which I've used while training and validating. Keep in mind there were ~35K files   but due to GitHub limitations I am only able to upload 1000 images. But the requirement can be satisfied by   implementing commands from instructions.txt

./datasets   <br />
  Alongwith synthetic folder, there are some files such as annotations, Jupyter Notebook to process them and   tfrecords.
  
./exported-model   <br />
  It contains different frozen graphs, but the one that I've used at the last is frozen_graph.pb.     It's not been generated using built-in export from aocr, It's been generated using Exporting and Reusing     Inference Graph AOCR.ipynb.


./static   <br />
  It's just a reference folder for storing temporaring image files for our web-app.
  
./text-renderer-master    <br />
  It's a github repo by user "Sanster" and can be located here : https://github.com/Sanster/text_renderer.   Some preprocessing needs to be done to add corpus into the ./text-renderer-master/data/corpus which is     not present currently in the repo due to upload limitations from GitHub. Steps to do that is mentioned     in instructions.txt.
 
./App_Home_Page.png and ./App_Predicted_Page.png   <br />
  It's an image of my Home Page and Predicted Page of the app. Referred from : https://cv-tricks.com/how-to/freeze-tensorflow-models/

  
./IITB-Assignment-Laxya Agarwal.pdf   <br />
  Report for the assignment
 
./Procfile   <br />
  For Heroku
  
./WEBAPP.ipynb   <br />
  Jupyter Version of  Web App

./aocr.log   <br />
  Log of AOCR training, validating, predicting
  
./app.py   <br />
  Web app, can be run using "python3 app.py" within the repo.
  
./instructions.txt    <br />
  Step by Step instructions to run the project
  
./exported/frozen_graph.py    <br />
  manually exported frozen graph

./my_run.sh TestImageFolderName OutputFileName   <br />
  It executes by passing TestImageFolderName and OutputFileName. It might get an error so use
  # "aocr predict --dirpath TestImageFolderName --out_file_name OutputFileName --max-prediction 23 --max-height 48 --max-width 960 -"
  
./requirements.txt    <br />
  For Heroku
 
./values1.txt    <br />
  Example file after executing my_run.sh TestImageFolderName values1
