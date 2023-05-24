# ACGAN
## Usage
运行根目录下aigc_mn.py

接口类文件aigcmn.py。实现接口类AiGcMn，类的初始化函数中完成模型加载等初始化工作。

接口类AiGcMn提供一个接口函数generate，该函数的参数是一个整数型n维tensor（n是batch的大小，每个整数在0~9范围内，代表需要生成的数字），输出是`n*1*28*28`的tensor（n是batch的大小，每个`1*28*28`的tensor表示随机生成的数字图像）。

运行main函数可以进行测试，其中内置了保存图片的功能，用于检测生成图像是否正确。

## TODO
* 修改文件，删除其中没有意义的函数（如parse_args）
* main函数中的保存图像函数路径与实际意义不符，不过只检验图片是否正确，所以懒得改了，有兴趣可以调一下
* 调整文件顺序，增加注释