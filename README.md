# done and todo

为了在自己服务器运行，安装tensorflow1.15版本
修改run_classifier.py 进finetune
主要是修改文件处理部分:
    找到main、添加任务、添加对应processor 类, processor中包含了：文件路径、label种类、读取方法等，照猫画虎
其中的processor就是task name
