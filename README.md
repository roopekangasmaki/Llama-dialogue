# Llama-dialogue

Here is one example of the Peft model summary compared to human summary:
![Screenshot 2025-02-18 232612](https://github.com/user-attachments/assets/d1742e60-1ab0-4439-b45a-97062ca5664c)
As can be seen, the Peft model misinterprets the situation and thinks the conversation concerns an invitation to birthday party, when the conversation is actually happening at a birthday party.

Here are a few more examples. Qualitatively both original model and peft model have their pros and cons. Original can be concise, but gets messed up often, while peft model is not always accurate, but is more informative.
![Screenshot 2025-02-18 234128](https://github.com/user-attachments/assets/5ab6b28e-286a-4a1e-b11b-004a12f9438d)

Here are rouge scores for both models. Neither of the models are that good, but peft model was slightly better than original model.
![Screenshot 2025-02-18 234538](https://github.com/user-attachments/assets/485f9fe0-c5dc-4010-901f-aa2c35d03e9c)

Errors encountered and fixes applied:
- Fixed an issue, where Hugging face sign up window didn't show up by changing interface_login to login
- Changed path to pretrained PeftModel from Kaggle format to local computer
- Increased print output width of Pandas dataframes

Snapshot of hugging face model and link
![Screenshot 2025-02-18 232117](https://github.com/user-attachments/assets/f360b36f-4eed-4a1b-a789-5d13886a7dba)
https://huggingface.co/RoopeK/TinyLlama-dialog-finetuned
