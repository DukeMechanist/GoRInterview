小测试：
===========================
## 按照下面的要求，依次实现一个小型无敌斩演示Demo：

1. 在场地中随机创建五位英雄（Resources里），位置范围是距离原点 4 米内（X，Z轴平面），朝向随机（forward在XZ平面内）
2. 在场地中随机创建20个怪物（Resources里），位置范围是以原点为中心的一个边长为 15 的正方形（X，Z轴平面），朝向随机（forward在XZ平面内），这些怪物中，有一个特殊的怪物，名字设为Boss。
3. Log，UI，两个模块，创建每个角色的时候，进行响应。
4. 实现主宰（Juggernaut）的无敌斩技能： 
   1. 用OnGUI在屏幕上绘制一个按钮，点击时，主宰开始释放无敌斩
   2. 开始释放技能时，Log，Sound，UI，三个模块对此作出响应。
   3. 找到距离英雄 8 米范围内的所有敌人
   4. 把敌人从近到远排序（排序算法要求自己实现）
   5. 排序完之后，把名字为Boss的怪物从列表里剔除
   6. 每 0.5 秒，主宰按照刚才排序的顺序，依次斩杀一个怪物，斩杀每个怪物的流程如下：
      1. 主宰移动到一个怪物身后距离1米处
      2. 移除怪物
      3. Log，Sound，UI，三个模块对此作出响应。
5. （选做）把工程上传到自己的Github，保存在一个新的分支上，把项目的地址发到email：hr@mechanist.co
6. （选做）如果不会使用Github，则把整个工程打包后，发到email：hr@mechanist.co

        
## Bonus：
1. 使用Quaternion
2. 模块之间不耦合
3. 斩杀时的表现