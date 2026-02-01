# F022 五种推荐算法之化妆品美妆推荐可视化系统vue+flask

> 完整项目收费，可联系QQ: 81040295 微信: mmdsj186011 注明从git来的，谢谢！
也可以关注我的B站： 麦麦大数据 https://space.bilibili.com/1583208775
> 
B站up账号:  麦麦大数据
关注B站，有好处！
编号:  F022
## 视频

[video(video-IRE0IpFi-1758179788295)(type-bilibili)(url-https://player.bilibili.com/player.html?aid=814702540)(image-https://i-blog.csdnimg.cn/img_convert/b2ac1d08e98b12f75c96a9f1e9e5b393.png)(title-炸天五种推荐算法之化妆品美容推荐系统大数据可视化Vue python flask)]

## 1 系统简介
系统简介：本系统是一个基于Vue.js前端框架和Flask后端框架的化妆品推荐系统，采用MySQL作为数据库存储爬取的化妆品数据。系统通过爬虫技术从多渠道获取化妆品信息，并存储到数据库中，为后续的推荐和分析提供数据支持。推荐模块集成了五种算法：UserCF（基于用户的协同过滤）、ItemCF（基于物品的协同过滤）、SVD（奇异值分解）、混合CF（结合多种协同过滤方法）以及混合CF+神经网络（融合协同过滤与深度学习）。系统还提供了丰富的数据分析功能，包括化妆品产地地图、品牌分析（通过花瓣图、柱状图、折线图等可视化形式展示）、店铺分析（仪表盘、花瓣图等）、以及化妆品介绍的词云分析。用户可以通过注册和登录功能管理个人信息，并根据推荐算法获得个性化的化妆品推荐。
## 2 功能设计
系统主要包含以下功能模块：

爬虫模块：从多渠道爬取化妆品数据并存储到MySQL数据库中，确保数据的完整性和实时性。
推荐系统模块：实现了UserCF、ItemCF、SVD、混合CF和混合CF+神经网络五种推荐算法，能够根据用户的历史行为和偏好提供个性化的化妆品推荐。
化妆品产地分析模块：通过地图可视化展示化妆品的产地分布，帮助用户了解不同地区的化妆品特点。
品牌分析模块：利用花瓣图、柱状图、折线图等形式展示品牌的市场表现、热度和用户偏好。
店铺分析模块：通过仪表盘、花瓣图等可视化工具分析店铺的销售数据和用户评价。
化妆品介绍分析模块：通过jieba分词和词云分析，提取化妆品介绍中的关键词，帮助用户快速了解产品特点。
用户模块：支持用户注册、登录和个人信息管理，为推荐系统提供用户行为数据。
通过这些功能模块的协同工作，系统能够为用户提供高效、精准的化妆品推荐服务，同时帮助用户深入了解化妆品的市场趋势和特点。
### 2.1系统架构图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b4dcb3955a4049949e232f1c9b682187.png)
### 2.2 功能模块图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f2a8f95c2f7b483598ba8ae635f7439d.png)
### 2.3 推荐算法
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/3e1e95385abd4596953de5b04738766b.png)
## 3 功能展示
### 3.1 登录 & 注册
登录注册做的是一个可以切换的登录注册界面，点击去登录后者去注册可以切换，背景是一个视频，循环播放。
登录需要验证用户名和密码是否正确，如果**不正确会有错误提示**。
注册需要**验证用户名是否存在**，如果错误会有提示。
### 3.2 主页
主页的布局采用了左侧是菜单，右侧是操作面板的布局方法，右侧的上方还有用户的头像和退出按钮，如果是新注册用户，没有头像，这边则不显示，需要在个人设置中上传了头像之后就会显示。
数据统计展示了系统内商品总数还有各个化妆品品类的商品数据的分析结果：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/3620bb87c2af4660830e4fe4c0519bd6.png)
### 3.3 推荐算法
**usercf**:
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b6a21e7331e2452b9c1825b82f9536ed.png)
**itemcf**:
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/53dbce6b3c0b49c8ae1f6eb68e1653bb.png)
**svd**:
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f91e5c0ff4944159a6fc9b0390582814.png)
**混合CF**:
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c111a5ba0b2c41ea9c7bc9e15e1eecd6.png)
**神经网络**：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/30e822bf9c00463186fb6f2f65f99863.png)
### 3.4 数据分析
品牌分析：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/34bba1ffeac74e23b4a3d08761ee4f3e.png)
店铺分析：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/52269409c4ff43b1a69894b23caf23aa.png)

产地地图：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/455e48241170497abf05971d3c885474.png)
词云分析：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/8039c91805d04b3e88228bac79dfab43.png)
## 4程序代码
### 4.1 代码说明
代码介绍：实现了一个基于MLP的化妆品推荐系统。首先，通过加载用户、产品和交互数据，合并特征并进行标准化处理。模型使用多层感知机（MLP）结构，包含两个隐藏层，分别使用ReLU激活函数，最后一层使用sigmoid函数进行二分类（点击或未点击）。模型训练使用adam优化器和二元交叉熵损失函数。推荐功能通过输入用户ID，生成个性化推荐列表，输出产品ID及其点击概率分数。代码结构清晰，适合化妆品推荐场景。
### 4.2 流程图

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/240277d848fc4b4fa82688a2253dabb5.png)

### 4.3 代码实例
```python

# 基于MLP的化妆品推荐算法

from sklearn.preprocessing import StandardScaler
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense
import numpy as np
import pandas as pd

# 1. 数据加载与预处理
def load_data():
    user_features = pd.read_csv("user_features.csv")  # 用户特征（如年龄、性别、购买历史）
    product_features = pd.read_csv("product_features.csv")  # 化妆品特征（如类别、价格、品牌）
    interaction_data = pd.read_csv("interaction.csv")  # 用户与产品的交互数据（如点击、购买）

    # 合并特征
    data = pd.merge(interaction_data, user_features, on="user_id")
    data = pd.merge(data, product_features, on="product_id")

    # 标准化处理
    scaler = StandardScaler()
    data[["age", "price"]] = scaler.fit_transform(data[["age", "price"]])

    # 特征和标签分离
    X = data.drop(["clicked", "user_id", "product_id"], axis=1)
    y = data["clicked"]  # 1表示点击，0表示未点击

    return X, y

# 2. 模型构建与训练
def train_model(X, y):
    model = Sequential()
    model.add(Dense(64, activation="relu", input_shape=(X.shape[1],)))
    model.add(Dense(32, activation="relu"))
    model.add(Dense(1, activation="sigmoid"))

    model.compile(optimizer="adam", loss="binary_crossentropy", metrics=["accuracy"])
    model.fit(X, y, epochs=10, batch_size=128, validation_split=0.2)

    return model

# 3. 生成推荐
def generate_recommendations(model, user_id, top_n=5):
    user_features = pd.read_csv("user_features.csv")
    product_features = pd.read_csv("product_features.csv")

    # 获取目标用户的特征
    user = user_features[user_features["user_id"] == user_id]
    products = product_features.drop("product_id", axis=1)

    # 合并用户和产品特征
    recommendations = pd.concat([user.drop("user_id", axis=1)] * len(products), ignore_index=True)
    recommendations = pd.concat([recommendations, products], axis=1)

    # 预测点击概率
    predictions = model.predict(recommendations)
    recommendations["score"] = predictions.flatten()

    # 排序并返回前N个产品
    return recommendations.sort_values("score", ascending=False).head(top_n)[["product_id", "score"]]

# 主函数
if __name__ == "__main__":
    X, y = load_data()
    model = train_model(X, y)
    recommendations = generate_recommendations(model, user_id=123)
    print("推荐结果:")
    print(recommendations)

```
