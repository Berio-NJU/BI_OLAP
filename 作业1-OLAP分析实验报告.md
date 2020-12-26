# 作业1-OLAP分析实验报告

## 1. 数据集合说明

Food Mart公司，1997年和1998年的数据库备份foodmart.bak

https://github.com/Berio-NJU/BI_OLAP.git

## 2. OLAP分析工具说明

- SQL Server 2019
- SQL Server Analysis Services
- SSMS
- Visual Studio 2017
- Excel

## 3. 分析过程

### 3.1 建立数据库

- 将FoodMart.bak导入SQL Server
- ![image-20201226153937060](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226153937060.png)

### 3.2 导入数据源

- 使用foodmart数据库向SSAS导入数据源
- ![image-20201226154246485](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226154246485.png)

### 3.3 建立数据源视图

- 引用分析需要的维表与事实表。
- 设置表的逻辑主键，并建立表的连接。
- 结果

![image-20201226154453538](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226154453538.png)

### 3.4 建立维表

- 使用数据源现有表建立维表。

![image-20201226154624598](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226154624598.png)

- 为每个维表建立层次结构
- ![image-20201226154746381](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226154746381.png)
- ![image-20201226154755518](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226154755518.png)
- ![image-20201226154808067](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226154808067.png)
- ![image-20201226154822317](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226154822317.png)
- ![image-20201226154858644](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226154858644.png)

### 3.5 建立数据仓库

- ![image-20201226155218831](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226155218831.png)

### 3.6 使用Excel进行分析

- 时间维度展开到The Day，Product维度展开到Product Department，按照总计的降序排列

- ![image-20201226161651767](C:\Users\Administrator.DESKTOP-CGIO78B\AppData\Roaming\Typora\typora-user-images\image-20201226161651767.png)

## 4. 分析结论和决策说明

### 4.1 分析结论

根据分析得到，Food，Drink，Non-Consumable三类中，销售额最高的分别是Canned Foods，Beverages，Household.

### 4.2 决策说明

根据分析结论，我们可以在超市的布局中，把Canned Foods，Beverages和Household类的商品放置在超市最显眼、最方便的地方，以便提高顾客的购物效率和超市的营业额。

