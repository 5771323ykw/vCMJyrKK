# 前言

欢迎来到我们的高校二手平台项目，该项目是基于SSM（Spring、Spring MVC、MyBatis）框架开发的一款方便高校学生进行二手物品交易的在线平台。在这里，学生们可以轻松发布自己的二手物品，也可以浏览和购买其他学生的二手物品。

# 内容介绍

本项目主要包括以下几个功能模块：用户模块、商品模块、交易模块和消息模块。用户模块提供了用户注册、登录、修改个人信息等功能；商品模块包括发布商品、浏览商品、搜索商品等功能；交易模块负责处理订单、支付和售后等操作；消息模块则为用户提供实时通知和交流的平台。

为了让用户有更好的体验，我们采用了Vue前端框架，实现了页面的快速加载和数据的双向绑定。同时，项目后端采用了Java语言和SSM框架，保证了系统的稳定性和可维护性。

# 技术介绍

- 语言：Java
- 使用框架：Spring、Spring MVC、MyBatis
- 前端技术：JS、Vue、CSS3
- 开发工具：IDEA/Eclipse
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven: apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

# 核心代码

以下是商品模块中的一个查询商品的方法：

```java
// 商品Service层
public List<Product> queryProductList(Product product) {
    // 调用MyBatis的Mapper接口查询商品列表
    return productMapper.queryProductList(product);
}

// 商品Mapper接口
public interface ProductMapper {
    List<Product> queryProductList(Product product);
}

// 商品Mapper.xml
<select id="queryProductList" parameterType="Product" resultType="Product">
    SELECT * FROM product
    <where>
        <if test="productName != null and productName != ''">
            AND product_name LIKE CONCAT('%', #{productName}, '%')
        </if>
        <if test="productType != null">
            AND product_type = #{productType}
        </if>
    </where>
</select>
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/342130/40/1971/71186/68c1aabfFb177dc14/e36abd934c66915e.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/324866/15/18573/5619/68c1aa96F0c3ee2f7/c97ffe460fcc5b9d.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/348725/32/1920/56588/68c1aa97Fca440727/05e0d26991ae5e9e.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/344041/6/1928/20639/68c1aa97F94822805/9b69fb9d034fa661.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/340002/16/9311/3406/68c1aa97F04c391ac/9f2a0edb159182a5.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/337693/24/9100/48111/68c1aa98Fdcf8b907/3996fe93f19698df.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/330857/23/11807/23191/68c1aa98F2ccfe588/1a8614ff7b631fea.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/329539/28/11919/32153/68c1aa98Ff4f788d0/f9b06bac72389ef2.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/349556/10/1977/66479/68c1aa98Ffb97a8c7/a5f0c21262866c14.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/331684/10/11600/46235/68c1aa99F9009522e/82218693034ac271.jpg)

