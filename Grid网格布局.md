# Grid 网格布局

## 1.   定义网格

![image-20220927201105863](assets/image-20220927201105863.png)

**网格定义比容器小**

![image-20220927201351950](assets/image-20220927201351950.png)

**子项比网格小**

![image-20220927201509847](assets/image-20220927201509847.png)

## 2. fr单位

![image-20220927202356096](assets/image-20220927202356096.png)

## 3. 合并网格及网格命名

使用命名方式定义网格区域， 需配合grid-area属性进行使用

![image-20220927203505684](assets/image-20220927203505684.png)

**缩写形式**

![image-20220927204555936](assets/image-20220927204555936.png)

## 4. 网格间隙及简写

用来设置元素行列之间的间隙大小

- grid-row-gap
- grid-column-gap 
- grid-gap



简写形式去掉了grid前缀， 分别为

- row-gap
- column-gap
- gap

![image-20220927205742519](assets/image-20220927205742519.png)

## 5. 弹性布局设置间隙

![image-20220927210258532](assets/image-20220927210258532.png)

## 6. 网格对齐方式及简写

- justify-items   水平方向, 取值为 start, center, end
- align-items   垂直方向, 取值为start, center, end
- place-items

默认值 stretch, 指定了子项在网格中的对齐方式

![image-20220927212831973](assets/image-20220927212831973.png)

缩写形式

![image-20220927213238138](assets/image-20220927213238138.png)



## 7. 整体在容器中的对齐方式

- justify-content， 水平方向， 取值为 start , center, end， space-between
- align-content   垂直方向， 取值为start, center, end
- place-content  简写形式 

默认值 是stretch, 指定了所有风格在grid容器中的对齐方式

![image-20220927213910810](assets/image-20220927213910810.png)

![image-20220927214217390](assets/image-20220927214217390.png)

![image-20220927214321984](assets/image-20220927214321984.png)

## 8. 显示网格与隐式网格

- grid-auto-flow                             取值 为 row 和column, 在行和列上产生隐式网格
- grid-auto-rows                            设置隐式网格的行高
- grid-auto-columns                      设置隐式网格列宽
