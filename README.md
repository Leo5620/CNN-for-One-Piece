# CNN-for-One-Piece
My first CNN try, to classify the images. 

##########环境依赖
python 3.7.3
tensorflow-gpu 1.7
numpy 1.16.4

##########直接测试步骤
1. 通过命令行进入当前目录

2. 输入python test_model.py指令进行测试，如果缺少环境则先添加环境

3. 得到输出

##########训练网络步骤
1. 安装tensorflow的gpu版本（数据集大小为6000张图，建议在gpu环境下运行）

2. 通过命令行进入当前目录

3. 如果不想覆盖原有的模型，则更改train_model.py文件中的model_path，将模型保存到新的目录

4. 输入python train_model.py指令进行训练

5. 等待模型训练

6. 得到精确度曲线则说明训练完成

7. 输入python test_model.py指令开始测试

8. 得到新模型的测试结果

##########对其他文件的说明
1. enhance_data.py
该文件用于增强数据集，初始目录为original_data下的指定文件夹，输出目录为enhanced_data的指定文件夹

2. image_change.py
该文件用于引入新的图片，可在testset/new_image目录下放置新的png图片，运行image_change.py，新的图片将会输出到testset，随后双击testset目录下的1.bat文件，将jpg后缀更改为png后缀，由此可以保证测试程序的运行。训练集也同样可以用该方法引入图片。

3. test_result_0.818.png
当前模型进行测试的结果

4. list.txt
完整的目录树

##########文件目录简略版
├─enhance_data.py            //增强数据

│  image_change.py            //改变新引入图片的模式

│  list.txt                   //完整的目录树

│  readme.md                  //help

│  test_model.py              //测试模型

│  test_result_0.818.PNG      //当前模型的测试结果

│  train_model.py             //训练模型
│  
├─enhanced_data               //增强后的数据集
│  ├─lufei
│  │      *.png
│  │      
│  ├─luobin
│  │      *.png
│  │      
│  ├─namei
│  │      *.png
│  │      
│  ├─qiaoba
│  │      *.png
│  │      
│  └─suolong
│          *.png
│          
├─original_data                //初始数据集
│  ├─lufei
│  │      *.png
│  │      
│  ├─luobin
│  │      *.png
│  │      
│  ├─namei
│  │      *.png
│  │      
│  ├─qiaoba
│  │      *.png
│  │      
│  └─suolong
│          *.png
│          
├─testset                       //测试数据集
│  │  1.bat                     //批量更改图片后缀
│  │  101.png
│  │  102.png
│  │  103.png
│  │  204.png
│  │  205.png
│  │  306.png
│  │  307.png
│  │  408.png
│  │  409.png
│  │  510.png
│  │  511.png
│  │  
│  └─new_image                   //存放新的测试图片
└─zengqiangmodel                 //当前模型
        checkpoint
        model.ckpt.data-00000-of-00001
        model.ckpt.index
        model.ckpt.meta




##########邮箱
846895620@qq.com
