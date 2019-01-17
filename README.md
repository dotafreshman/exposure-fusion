# exposure-fusion
## example.m是文件的top——在里面，先load.m，后exposure.m()
* exposure下，又有`contrast`, `saturation`, `well-expose`三成员，以及`gaussian_pyramid`, `laplace_pyramid` 2成员  
  * pyramid——一个cell，每一格是W/I用downsample迭代滤过  
  * exposure流程
    mermaid
    graph LR
      A[图像]==3成员==>B[权重W]==pyramid==>B[pryW]==组合==>B[pry]==reconstruct==>B[图像]
  
  
  
Implementation of Exposure Fusion in Matlab, as described in:

  "Exposure Fusion",
  Tom Mertens, Jan Kautz and Frank Van Reeth
  In proceedings of Pacific Graphics 2007

  "Exposure Fusion: A Simple and Practical Alternative to High Dynamic Range Photography. "
  Tom Mertens, Jan Kautz and Frank Van Reeth
  In Computer Graphics Forum, 28 (1) 161 - 171, 2009

This code was originally written by Tom Mertens at Hasselt University, August 2007.
Uploaded to GitHub in February 2015

Author and main contact: Tom Mertens, tom.mertens@gmail.com


To get started, go to 'example.m'.

Subdirectory 'house' contains a sample dataset (photos by Min H. Kim, as used in the paper)
