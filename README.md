# To use it Locally 

1. Just Make Sure to  **Restart your kernel**  every time to see every model Performance seperately
2. For GLOVE Embeddings , Download 25 dimensional 27 Billion tokens twitter text file
3. You can download it from **https://huggingface.co/stanfordnlp/glove/resolve/main/glove.twitter.27B.zip**
4. If you dont have dedicated GPU , You can remove the first cell and can just import tensorflow


# Model Architecture 

 Layer (type)                Output Shape              Param #   
=================================================================
 embedding_2 (Embedding)     (None, None, 25)          335000    
                                                                 
 bidirectional_4 (Bidirectio  (None, None, 50)         10200     
 nal)                                                            
                                                                 
 bidirectional_5 (Bidirectio  (None, 50)               15200     
 nal)                                                            
                                                                 
 dense_4 (Dense)             (None, 24)                1224      
                                                                 
 dense_5 (Dense)             (None, 1)                 25        
                                                                 
                                                                
=================================================================
Total params: 361,649
Trainable params: 26,649
Non-trainable params: 335,000

**Non-trainable params are the vector embeddings initialised from GLove**