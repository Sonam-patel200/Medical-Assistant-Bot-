Description of the approach used to tackle the problem:  
An encoder/decoder model that will take the data that we provide and output our response using the techniques of machine translation.

 Assumptions made during model development and training :

 
 All tokens in the input sequence are treated equally, regardless of their position or relevance to the current decoding step.
The model assumes that all relevant information needed to generate the output sequence is captured in the fixed-length representation obtained from the encoder. Therefore, it may struggle with capturing long-range dependencies or understanding context that spans across distant parts of the input sequence.
The fixed-length representation obtained from the encoder must compress all relevant information from the input sequence into a single vector. 

 Model's performance:
 Used Test Loss metric to evaluate performance. The use of Test Loss for evaluating model performance is fundamental because it provides a clear, quantitative, and objective measure of how well a model is likely to perform on new, unseen data. It helps in understanding generalization, guiding model development, and ensuring that the model is robust and reliable for real-world applications.

 Strengths of the Model: 
 Good Performance on Simple Tasks: For simple sequence-to-sequence tasks with relatively short input and output sequences and limited long-range dependencies, the model without attention can perform reasonably well.
  The absence of attention simplifies the training process as well.

   Weaknesses:
   The fixed-length representation obtained from the encoder compresses all information from the input sequence into a single vector and  limit the model's ability to understand and capture the full context of the input.
   The model without attention assumes fixed-length input and output sequences, making it less flexible in handling variable-length input and output sequences. 



   Potential improvements or extensions to the solution, such as refining the model
 architecture: 
 
 Finding a model which is trained on medical data then fine tune it on this QA dataset, this could improve the   overall performance and robustness of the system.
 

  

 
