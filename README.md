# Cartoonizer

> Convert images and videos into a cartoon!

The webapp is deployed here - https://cartoonize-lkqov62dia-de.a.run.app
<div style="text-align:center"><img height="100" alt="Powered by Algorithmia" style="border-width:0" src="static/sample_images/algorithmia.jpeg" /></div>

You can find a writeup on this webapp's architecture [here](https://medium.com/@Niraj_pandkar/how-we-built-an-inexpensive-scalable-architecture-to-cartoonize-the-world-8610050f90a0)!

---

## Installation Using [Google Colab](https://colab.research.google.com/drive/1oDhMEVMcsRbe7bt-2A7cDsx44KQpQwuB?usp=sharing)

### Using [Google Colab](https://colab.research.google.com/drive/1oDhMEVMcsRbe7bt-2A7cDsx44KQpQwuB?usp=sharing)
1. Clone the repository using either of the below mentioned way:
   - Using Command:
        - Create a new Notebook in Colab and in the cell execute the below command.  
        
        ```
         ! git clone https://github.com/experience-ml/cartoonize.git
        ```
        **Note:** Don't forget to add `!` at the beginning of the command
        
    - From Colab User Interface
 ```
        Open Colab
            └── File
                 └── Open Notebook
                          └── Github
                                └── paste the Url of the repository
 ```
 Note :  Before running the application change the runtime to GPU for processing videos but you for images CPU shall also work just fine.
 ```
            Runtime
               └── Change runtime type
                           └── Select GPU
 ```
2. After cloning the repository navigate to the `/cartoonize` using below command in the notebook cell:

   ```
   %cd cartoonize
   ```
3. Run the below commands in the notebook cell to install the requirements. 

   ```
   !pip install -r requirements.txt
   ```
   
4. config your pyngrok to solve NAT Traversal(ngrok account registration in advance needed).

  ```
  !ngrok authtoken YOUR_NGROK_TOKEN
  ```
   
5. Launch the flask app on ngrok

   ```
   !python app.py
   ```
   
6. just click the link app.py provides or connect to colab in RESTful requests.

  ```
  POST http://xxxx-xx-xxx-xxx-xxx.ngrok.io/cartoonize
  ```

#### Note : Sample [Google Colab Notebook](https://colab.research.google.com/drive/1oDhMEVMcsRbe7bt-2A7cDsx44KQpQwuB?usp=sharing) for reference

---

## License

1. Copyright © Cartoonizer ([Demo webapp](https://cartoonize-lkqov62dia-de.a.run.app/))

    - Authors: [Niraj Pandkar](https://twitter.com/Niraj_pandkar) and [Tejas Mahajan](https://twitter.com/tjdevWorks).

    - Licensed under the [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode) 
    - Commercial application is prohibited by license


2. Copyright (C) Xinrui Wang, Jinze Yu. ([White box cartoonization](https://github.com/SystemErrorWang/White-box-Cartoonization))
    - All rights reserved. 
    - Licensed under the CC BY-NC-SA 4.0 
    - Also, Commercial application is prohibited license (https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
