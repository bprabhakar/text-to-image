# AttnGAN Inference via Pre-trained Model

## Running inference
There are three steps involved.
1. Create the container (optionally choose the cpu or gpu dockerfile: 
   ```
   docker build -t "attngan" -f dockerfile.cpu .
   ``` 
2. Run the container (replace the key's with the appropriate blob storage location as well as App Insights Key): 
    ```
    docker run -it --name attngan -p 8888:8888 attngan bash
    ```
3. Run the jupyter notebook. 

# Credits
All the code has been borrowed from https://github.com/taoxugit/AttnGAN.
This repo just simplifies the evaluation api into a single Jupyter notebook instead of hosting on Azure.


