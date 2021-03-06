cv.js
==========

## 简介

cv.js是一个用于图像处理的前端JS库，较完整的保留了图像处理算法本身，没有让js&canvas等语言因素影响算法的实现，希望能帮助到其他自学图形图像的同学们。

## 现有处理方式

- Gray：灰度处理
- Gauss：高斯模糊，有标准版和默认版。标准版是按照两次一维高斯卷积实现的，支持卷积半径和sigma参数的设定；默认版是按照3*3的高斯核直接做卷积实现的
- Bilateral：双边滤波，支持radius、sigma1、sigma2参数修改
- Laplace of Gauss：LoG边缘提取
- Sobel：Sobel边缘提取
- Difference of Gauss：DoG边缘提取
- Canny：Canny边缘提取
- Cartoon：卡通效果滤镜
- ColorConvert：lab、xyz、rgb色彩空间转换

## 后续

图形图像的学习是永无止境的，后续会添加Harris角点提取，以及图像匹配的处理进来。

## DEMO

- 访问目录中`example.html` 或 `index.html`，每次切换图片需要点击OK键
- 直接预览[DEMO](http://naixor.github.io/cv/)

## 使用

可参照 `example.html` 或 `index.html` 使用

## 初始化

- 需要先安装`npm`和`bower`，执行`npm install`然后`bower install`
- `npm init`

## 打包压缩

`grunt`

## 测试

- 执行`grunt test`，目录中后会生成一个名为`unit-test.html`的文件
- `php -S localhost:8080`
- 打开浏览器访问`http://localhost:8080/unit-test.html`，或者Mac下直接命令行执行`open http://localhost:8080/unit-test.html`