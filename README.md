## BERT Masked Language Model with Attention Visualization  

# Background    
One way to create language models is to build a Masked Language Model (MLM), where a language model is trained to predict a “masked” word that is missing from a sequence of text. BERT (Bidirectional Encoder Representations from Transformers) is a transformer-based language model developed by Google, which was trained using this approach: the model predicts masked words based on surrounding context words.  

BERT uses a transformer architecture and employs an attention mechanism to understand language. In the base BERT model, the transformer consists of 12 layers, with each layer having 12 self-attention heads, resulting in a total of 144 self-attention heads.  

This project has two main parts:  

- **Masked Language Model**: Using the Hugging Face Transformers library to write a program that uses BERT to predict masked words.
- **Attention Visualization**: Generating diagrams that visualize the attention scores for each of the 144 attention heads, helping us analyze what BERT’s attention heads focus on while understanding natural language.

# Features  
Predicts masked words in a given input text using BERT.  
Generates visual diagrams of attention scores for each attention head in the model.  
Visualizations are saved as PNG files for further analysis.  

# Example Output
When running the program, if the input is :
**The cat sat on the [MASK] and looked around., the output might include predictions like:** 

        The cat sat on the mat and looked around.  
        The cat sat on the rug and looked around.  
        The cat sat on the ground and looked around.  
        
Additionally, you will find PNG files named Attention_Layer1_Head1.png, Attention_Layer1_Head2.png, etc., in your working directory, visualizing the attention weights.  
![Attention_Layer1_Head1](https://github.com/user-attachments/assets/3c6e502a-f1b7-49ec-9c8e-8640f0ce5fff)
![Attention_Layer1_Head2](https://github.com/user-attachments/assets/0294aa6a-2c38-4551-bc43-18194af45f02)
![Attention_Layer1_Head3](https://github.com/user-attachments/assets/af364048-318f-4001-9bd7-65b2b47c5ec1)

# License  
This project is licensed under the MIT License. Feel free to modify and use the code as per your needs!  
