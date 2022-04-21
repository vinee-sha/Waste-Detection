# Waste-Detection
Waste Detection is a project which detects the waste into metal and plastic, bio, paper, glass, non-recyclable, other and unknown. YOLOv5 pre-trained algorithm is used in this project.

### DATASET :
Dataset Link: [Dataset](https://drive.google.com/drive/folders/1IJSFBPSt4uXKFZ4d4CUNkQwkLia3JIj7?usp=sharing)    
Datasets of Bio, Metal&Plastic, Paper, Glass, Non-Recyclable, and Other&Unknown are present in the Dataset separately. Each Dataset contains images and labels which are divided into train and test.     
It also contains a file - data.yaml in which all the class names are present.

### RUN THE PROJECT :
Get all the data from the GitHub, Open Command prompt or any other Terminal and run the command :    
  - git clone https://github.com/vinee-sha/Waste-Detection.git    
All the trained weights and the YOLO data are present in YOLOv5 Folder. Move to the YOLOv5 folder in the git using the commands :    
&nbsp;  \$cd Waste-Detection   
&nbsp;  \$cd YOLOv5    
Install all the modules and requirements that are needed to run the project with the command :   
&nbsp;  \$pip install -qr requirements.txt     
To test the weights, use the images and videos in the images folder under YOLOv5 or insert any images and videos for testing into the images folder and run the test using the command :    
&nbsp;  \$python detect.py --weights weights/Bio.pt weights/Glass.pt weights/Paper.pt weights/Metal-Plastic.pt --img 640 --source images/IMAGE_NAME    
The results are stored into yolov5/runs/detect/exp as mentioned in the output after running the previous command.    
