# BERT - NIPS Abstract  

### Prepare Data  
`python prepare_data.py --data_dir ../data/sentence_ordering_data/nips/ --out_dir ../output/nips_data/ --task_name nips`  

### Train the Model  
`python bert_classifier/model.py --data_dir ../output/nips_data/ --output_dir ../output/trained_models/nips_bert/ --do_train --do_eval --evaluate_during_training --per_gpu_train_batch_size 32 --per_gpu_eval_batch_size 16`  

### Test  
`python bert_classifier/model.py --data_dir ../output/nips_data/ --output_dir ../output/trained_models/nips_bert/checkpoint-6000/ --do_test --per_gpu_eval_batch_size 16`  


### Evaluate Results  
`python topological_sort.py --file_path ../output/nips_data/test_results.tsv`


# BERT - AAN Abstract 

### Prepare Data  
`python prepare_data.py --data_dir ../data/sentence_ordering_data/aan/ --out_dir ../output/aan_data/ --task_name aan`  

### Train the Model  
`python bert_classifier/model.py --data_dir ../output/aan_data/ --output_dir ../output/trained_models/aan_bert/ --do_train --do_eval --evaluate_during_training --per_gpu_train_batch_size 32 --per_gpu_eval_batch_size 16`  

### Test  
`python bert_classifier/model.py --data_dir ../output/aan_data/ --output_dir ../output/trained_models/aan_bert/checkpoint-18000/ --do_test --per_gpu_eval_batch_size 16`  


### Evaluate Results  
`python topological_sort.py --file_path ../output/aan_data/test_results.tsv`


# BERT - SIND Captions 

### Prepare Data  
`python prepare_data.py --data_dir ../data/sis/ --out_dir ../output/sind_data/ --task_name sind`  

### Train the Model  
`python bert_classifier/model.py --data_dir ../output/sind_data/ --output_dir ../output/trained_models/sind_bert/ --do_train --do_eval --evaluate_during_training --per_gpu_train_batch_size 32 --per_gpu_eval_batch_size 16`  

### Test  
`python bert_classifier/model.py --data_dir ../output/sind_data/ --output_dir ../output/trained_models/sind_bert/checkpoint-14000/ --do_test --per_gpu_eval_batch_size 16`  


### Evaluate Results  
`python topological_sort.py --file_path ../output/sind_data/test_results.tsv`

