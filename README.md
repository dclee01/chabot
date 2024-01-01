# chabot
Ada chatbot
1. Decompress file 20231207_ada_chatbot
2. Download the pychram, python3.0, then open the file 20231207_ada_chatbot
3. Create the python virtual environment
4. Run the python virtual environment in a terminal: .\venv\Scripts\activate.ps1
5. Enter python app.py, system will tell you what files need to be installed, then install all file you need: pip install xxx
6. When you download werkzeug meet problem, make sure your werkzeug version is 2.3.7 
7. If error again, come to flask_uploads.py file, error like this: File "D:\2023 Fall\ICSI-499\ada_chatbot\venv\lib\site-packages\flask_uploads.py", line 26, in <module> from werkzeug import secure_filename, FileStorage
8. Go tofind line 26, Delete the code in line 26 and replace with: 
from werkzeug.utils import secure_filename
from werkzeug.datastructures import  FileStorage
9. The code is runing in the local, so make sure your computer have gpu, you need download a CUDA Toolkit, use your gpu to run it in local, don't forget download the torch
10. After all the required files are downloaded, type python app.py in terminal again, the required model files will be download, wait for the model files to be downloaded and type python app.py in terminal, wait for a while, you will see the program running successfully, click Running on http://127.0. 0.1:5000, welcome to ada chatbot!
