install anaconda,(Be sure to include conda in path directory) 
create a new folder named chatbot,  
inside the folder open command prompt 


type following command in order
```
conda create --name rasa python==3.8
conda activate rasa
conda install tensorflow
pip install --upgrade tensorflow
pip install rasa
```
In pip instal rasa they will ask you for directory give the path to your chatbot folder

Open chatbot folder and paste all the files provided in git inside the botdata folder(download raw file by option on top right conner), also while pasting be sure to replace files and folder instead of seperatly pasting it

inside command prompt type:

`rasa train`

In another command prompt tab type:
`conda activate rasa`
`rasa run actions`

Now you can use chatbot in command prompt itself by typing(in previously opened tab):

`rasa shell`

If you want to train my model further and know it's working just type 

`rasa interactive`


