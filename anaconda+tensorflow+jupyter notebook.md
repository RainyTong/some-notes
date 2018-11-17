# Mac上Anaconda+Tensorflow+Jupyter notebook使用

> 搞了半天终于搞定了。。。记录一下安装过程

- before 安装Anaconda: 已有tensorflow，python3.6， jupyter notebook.
然而无法在jupyter notebook上面使用tensorflow

- then 安装 Anaconda： 
  1. 在Anaconda下用`conda create -n tensorflow python=3.6`命令创建了tensorflow环境
  2. `source activate tensorflow #激活tensorflow环境`
  3. `conda install ipython`
    then enter `which ipython`, you can see `anaconda3/envs/tensorflow/bin/ipython`，表明ipython位于tensorflow之下
  4. `conda install jupyter`
    then enter `which jupyter`, you can see `/anaconda3/envs/tensorflow/bin/jupyter`，表明jupyter位于tensorflow之下
  5. 这时输入`jupyter notebook`发现`import tensorflow`还是会报错，显示没有此module (在tensorflow环境下运行python也无法import tensorflow)
   
     Solution：`conda install tensorflow`
  6. Successfully imported tensorflow!!! :wink:


- 运行流程：
```
wangyutong$ source activate tensorflow
(tensorflow)wangyutong$ jupyter notebook
(tensorflow)wangyutong$ source deactivate
```


