# ����Ҷ�任
## [����Ҷ�任����������](https://zh.m.wikipedia.org/zh-cn/����Ҷ�任)
����Ҷ�任��һ��Ӧ�÷�Χ�ǳ����һ���źŷ�����������Ҫ�����ǽ��źŴ�ʱ��任��Ƶ��
��������������Ϸ������еĶ�̬ͼ��ʾ����һ�ֽ��źŷֽ�Ϊ���Ҳ������Ҳ����Ӻ�������ʾ�ض���Ƶ�ʵ����Ҳ�������
���ĸ�ֵ��������������ͼ��Ƶ�ף�������Դ�źŵ�������Ϣ�����Ǵ洢�ռ������ȴ�ܴ����٣�
## һЩ�����Ը���Ҷ�任�Ĳ���
* ����Ҷ�任�����ƽ�ƾ���ͼ��ķŴ����
* ����΢�ֹ�ϵ���Կ��ٵõ�ͼ����ݶ�
* ������������˲�
## ���򲿷ֺ������
* ��ȡ����Ҷ�任�ĺ��ʵĴ�С
```c++
getOptimalDFTSize(int vecsize)
```
��Ϊ���㸵��Ҷ����ʱ��ѡȡ2���ݴη���С�ľ����ܹ������ٵ����㣬�ò�����ȡ��һ�����ڼ��㸵��Ҷ�任�ĺ��ʵ��ݴ�N��N����
����ڶԸ��������ݴ�С��ȡ2Ϊ�׵Ķ�����
* ��ͼ���ؿ�һ���Ĵ�С
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
��������ֱ�Ϊ���������ݡ�������ݡ����������ĸ�������ؿ�Ĵ�С���ؿ����͡��ؿ������ֵ
* Ϊͼ�����ͼ��
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
�˺����������ǽ��������ϲ�Ϊһ�����ж���ͨ��������
* ��ͼ�����dft�任
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
* ��ͼ�����
```c++
void cv::split 
(
const Mat & 
src, 


Mat * 
mvbegin 

)

```
* ��ģ
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
* ����ʮΪ�׵Ķ���
```c++
softfloat cv::log 
(
const softfloat & 
a
)
```
һ�����������������һ�����������飬һ�����������