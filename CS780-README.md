# Direct Preference Optimization
A document to track our experiments using this repo.

I included a file `config/gemma-2b.yaml` which includes the config to run DPO on gemma-2b model from huggingface and see the results. 
```bash
python -u train.py model=gemma-2b datasets=[hh] loss=sft exp_name=google_dpo_gemma2b gradient_accumulation_steps=2 batch_size=64 eval_batch_size=32 trainer=BasicTrainer sample_during_eval=false
```