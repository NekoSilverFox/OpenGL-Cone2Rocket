<!-- SPbSTU 报告起始 -->

<div align="center">
  <!--<img width="250px" src="https://raw.githubusercontent.com/NekoSilverFox/NekoSilverfox/403ab045b7d9adeaaf8186c451af7243f5d8f46d/icons/new_logo_spbstu_ru.svg" align="center" alt="new_logo_spbstu_ru" />  新式 π logo -->
  <img width="250px" src="https://github.com/NekoSilverFox/NekoSilverfox/blob/master/icons/logo_building_spbstu.png?raw=true" align="center" alt="logo_building_spbstu" /> <!-- 研究型大学 logo -->
  </br>
  <b><font size=3>Санкт-Петербургский политехнический университет Петра Великого</font></b>
  </br>
  <b><font size=2>Институт компьютерных наук и технологий</font></b>
  </br>
  <b><font size=2>Высшая школа программной инженерии</font></b>
</div>


<div align="center">
<b><font size=6>通过图元着色器改变形状</font></b>


[![License](https://img.shields.io/badge/license-Apache%202.0-brightgreen)](LICENSE)

</div>
<div align=left>
<div STYLE="page-break-after: always;"></div>
<!-- SPbSTU 报告结束 -->


[toc]



# 项目说明

- 这个项目旨在通过演示三维物体形状的变化来展示OpenGL图形编程的能力。项目使用Qt框架中的OpenGL库进行开发，并实现了从一个正方形平面到联盟号火箭形状的逐步转换。这种三维图形转换功能是通过在OpenGL内核模式下重新编写几何着色器实现的。在项目开发过程中，实现了以下功能：

    - 照明：使用OpenGL库中的光照模型，通过设置光源、光照强度和物体表面属性来模拟真实世界中的光照效果。
    - 纹理贴图：通过在物体表面贴上纹理图像来增强渲染效果，使物体看起来更真实、更具有细节。
    - 冯氏光照：使用冯氏光照模型对物体进行渲染，以模拟真实世界中的光照效果，并使物体看起来更加真实。

    此项目对于学习OpenGL图形编程和三维图形的变换非常有帮助，同时还能够为有关三维建模和可视化的应用提供基础。



效果如下：

## 过程详解

1. 首先，方形平面被转化为金字塔的形状

    ![image-20230323010415016](doc/pic/image-20230323010415016.png)

    ![image-20230323010430144](doc/pic/image-20230323010430144.png)

    ![image-20230323010434594](doc/pic/image-20230323010434594.png)

    ![image-20230323010437161](doc/pic/image-20230323010437161.png)

    

2. 将金字塔的底座拉伸成房子的形状

    ![image-20230323010442886](doc/pic/image-20230323010442886.png)

    ![image-20230323010449336](doc/pic/image-20230323010449336.png)

    

3. 继续拉伸下表面，增加椎体下部的顶点数量。经过这样的转变，它将呈现出铅笔的形状（火箭体）

    ![image-20230323010527488](doc/pic/image-20230323010527488.png)

    ![image-20230323010530054](doc/pic/image-20230323010530054.png)

    ![image-20230323010532744](doc/pic/image-20230323010532744.png)

4. 最后，加入四个助推器，使其看起来像联盟号火箭

    ![image-20230323010541365](doc/pic/image-20230323010541365.png)

    ![image-20230323010543829](doc/pic/image-20230323010543829.png)

    

