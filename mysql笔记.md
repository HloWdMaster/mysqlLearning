- 检索数据

  ```
  distinct 范围是所有列
  ```

- 数据过滤

  ```
  值为NULL的数据不会被筛选 需要加上 IS NULL 判断
  
  ```

- 组合过滤

  ```
  AND
  
  OR
  
  IN
  IN（？，？ ）  ==>  OR 
  IN 可以包含select子句
  
  NOT
  否定之后所跟的任何条件
  NOT IN（？，？）
  ```

- 通配符过滤

  ```
  LIKE 匹配一整列
  " % "	任意字符出现任意次数
  " _ "	匹配任意单个字符
  ```

- 正则表达式进行匹配

  ```
  REGEXP (BINARY) 使用BINARY时区分大小写
  WHERE colname REGEXP ""
  
  \\\ 匹配 \
  ```

- 计算字段

  ```
  拼接函数  Concat()
  去除右边多余空格	RTrim()
  去除左边多余空格	LTrim()
  别名 字段或值的替换名 用 as 
  
  ```

- 时间处理函数

  ```
  CURDATE()	当前日期
  CURTIME()	当前时间
  NOW()	当前日期+时间
  
  ```

- 聚集函数

  ```
  AVG()	返回某列的平均值
  COUNT()	返回某列的行数
  MAX()	返回某列的最大值
  MIN()	返回某列的最小值
  SUM()	返回某列值之和
  ```

- 数据分组

