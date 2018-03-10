# 傅里叶变换
## [傅里叶变换的物理意义](https://zh.m.wikipedia.org/zh-cn/傅里叶变换)
傅里叶变换是一个应用范围非常广的一种信号分析方法，主要作用是将信号从时域变换到频域
。代表的意义如上方链接中的动态图所示，是一种将信号分解为正弦波和余弦波叠加后，用来表示特定的频率的正弦波或余弦
波的赋值，这样画出来的图叫频谱，包含了源信号的所有信息，但是存储空间的内容却能大大减少！
## 一些常见对傅里叶变换的操作
* 傅立叶变换后进行平移就是图像的放大操作
* 根据微分关系可以快速得到图像的梯度
* 卷积特性用来滤波
## 程序部分函数解读
* 获取傅里叶变换的合适的大小
```c++
getOptimalDFTSize(int vecsize)
```
因为计算傅里叶级数时，选取2的幂次方大小的矩阵能够更快速地运算，该操作是取得一个用于计算傅里叶变换的合适的幂次N（N大于
或等于对该输入数据大小的取2为底的对数）
* 将图像拓宽一定的大小
```c++
void cv::copyMakeBorder 
(
InputArray 
src, 


OutputArray 
dst, 


int 
top, 


int 
bottom, 


int 
left, 


int 
right, 


int 
borderType, 


const Scalar & 
value = Scalar() 

)

```
输入参数分别为：输入数据、输出数据、上下左右四个方向的拓宽的大小、拓宽类型、拓宽区域的值
* 为图像添加图层
```c++
void cv::merge 
(
const Mat * 
mv, 


size_t 
count, 


OutputArray 
dst 

)
```
此函数的作用是将多个数组合并为一个具有多条通道的数组
* 对图像进行dft变换
```c++
void cv::dft 
(
InputArray 
src, 


OutputArray 
dst, 


int 
flags = 0, 


int 
nonzeroRows = 0 

)
```
* 将图层分离
```c++
void cv::split 
(
const Mat & 
src, 


Mat * 
mvbegin 

)

```
* 求模
```c++
void cv::magnitude 
(
InputArray 
x, 


InputArray 
y, 


OutputArray 
magnitude 

)
```
* 求以十为底的对数
```c++
softfloat cv::log 
(
const softfloat & 
a
)
```
一般输入参数有两个，一个是输入数组，一个是输出数组