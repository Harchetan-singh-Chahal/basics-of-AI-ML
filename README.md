# basics-of-AI-ML
Includes concepts learn day to day 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
# create tokenizer tokenizer = AutoTokenizer.from_pretrained(model_checkpoint, add_prefix_space=True)
# add pad token if none exists
if tokenizer.pad_token is None:
  tokenizer.add_special_tokens({'pad_token': '[PAD]'})
model.resize_token_embeddings(len(tokenizer))


1)add_prefix_space=True
