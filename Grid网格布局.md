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

**指定在显示网格之外的隐式网格，如何排列及尺寸大小**

- grid-auto-flow                             取值 为 row 和column, 在行和列上产生隐式网格
- grid-auto-rows                            设置隐式网格的行高
- grid-auto-columns                      设置隐式网格列宽

![image-20220928195505990](assets/image-20220928195505990.png)

**以上： 1，2，3 占的是显示网格， 4，5 占的是隐式网格**



![image-20220928195746611](assets/image-20220928195746611.png)

![image-20220928200458631](assets/image-20220928200458631.png)

在列上产生隐式网格， 默认是行上

![image-20220928200639914](assets/image-20220928200639914.png)

**指定在列上产生隐式网格**

![image-20220928200724900](assets/image-20220928200724900.png)



**自适应列布局**

![image-20220928201137351](assets/image-20220928201137351.png)

**紧密排列**

![image-20220928201409428](assets/image-20220928201409428.png)

![image-20220928201511060](assets/image-20220928201511060.png)



## 9. 基于线的元素放置

- grid-column-start
- grid-column-end
- grid-row-start
- grid-row-end

### 8.1 显示line number

![image-20220928202515135](assets/image-20220928202515135.png)

### 8.2 指定基于线的停靠位置

![image-20220928202706586](assets/image-20220928202706586.png)



![image-20220928203102745](assets/image-20220928203102745.png)

![image-20220928203329514](assets/image-20220928203329514.png)

### 8.3 span的用法

![image-20220928203558975](assets/image-20220928203558975.png)

![image-20220928203654328](assets/image-20220928203654328.png)

### 8.4 线的命名

![image-20220928204335340](assets/image-20220928204335340.png)

### 8.5 简写操作

- grid-row
- grid-column

基于线对应位置的缩写方式，通过 `/` 分割

![image-20220928204718191](assets/image-20220928204718191.png)

### 8.6 grid-area 

grid-row-start , grid-column-start, grid-row-end, grid-column-end 的缩写， 以及额外支持 grid-template-areas设置的网格名称

![image-20220928205200466](assets/image-20220928205200466.png)

### 8.7 子项的对齐方式

- justify-self
- align-self
- place-self

跟place-item用法相同， 只不过是操作指定子项

![image-20220928205653906](assets/image-20220928205653906.png)

## 10. repeat() 和 minmax()

### 10.1 repeat() 简写

![image-20220928210156626](assets/image-20220928210156626.png)



### 10.2 auto-fill 自动生成网格

![image-20220928210451501](assets/image-20220928210451501.png)

### 10.3 minmax() 方法， 设置最小和最大值的范围

![image-20220928211000963](assets/image-20220928211000963.png)

![image-20220928211151295](assets/image-20220928211151295.png)

### 10.4 根据分辨率，调整排列个数

![image-20220928211813817](assets/image-20220928211813817.png)

## 11. 比定位更方便的叠加布局

![image-20220928212938399](assets/image-20220928212938399.png)

## 12. 多种组合排列布局

