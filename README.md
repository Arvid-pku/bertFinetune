# done and todo

为了在自己服务器运行，安装tensorflow1.15版本
修改run_classifier.py 进finetune
主要是修改文件处理部分:
    找到main、添加任务、添加对应processor 类, processor中包含了：文件路径、label种类、读取方法等，照猫画虎
其中的processor就是task name


# 使用序列标注finetune

工程在BERT-NER
命令行：
CUDA_VISIBLE_DEVICES=1,2 python run_ner.py --data_dir=data/ --bert_model=bert-base-chinese --task_name=ner --output_dir=out_base --max_seq_length=128 --do_train --num_train_epochs 45 --do_eval --warmup_proportion=0.1

可以修改读取方式等，阅读run_ner.py
输出模型在outbase