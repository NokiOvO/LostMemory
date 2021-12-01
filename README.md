# LostMemory
腾讯游戏学院--光子大作业  LostMemory

微云链接：https://share.weiyun.com/FdLaZfG7

一、游戏大厅

（1）单人游戏    --全部实现

（2）局域网游戏（进阶选项)  --基本全部实现 （基于Session通信）

   1.创建房间,设置房间名字和最大人数  --实现
    
   2.搜索房间，显示房间列表  --实现
    
   3.玩家可以加入某个房间，所有人准备后房主开始游戏 --实现
    
   4.加入带有密码的房间 --未实现


二、战斗对局

（1）流程相关  --全部实现

  1.开始游戏展示loading图，倒计时10秒，倒计时结束开始刷新怪物  --实现 
  
  2.每过若干时间刷新一波怪物 --实现  
  
  3.怪物刷新完毕，守护NPC存活则所有玩家胜利；守护NPC被打爆，所有玩家失败  --实现  
  
  4.胜利/失败都会弹出当局结算界面，记录小队所有成员的游戏信息，如击杀、死亡数等等，可以点击按钮返回  --实现 （使用类似组播的方法，在服务器For循环调用每个Player Controller的本地游戏结束方法）  

（2）主角相关  --全部实现

  1.主角可以空手近战攻击，也可以拾取枪支来射击  --实现
  
  2.主角可以拾取枪械，可以拾取BUFF --实现
  
  3.具有主角属性面板，显示角色血量、武器，所带的BUFF，近战和持枪显示不同的按钮和UI --实现 
  
  4.显示小队列表，实时展示每个小队成员的名字和血量（进阶选项） --实现 (小队UI从Game State中的Player Array获取更新玩家信息)
  
  5.主角被击杀播放死亡动画，倒计时3秒后复活；复活具有次数，若次数用光，则判断游戏失败 --实现


（3）枪械相关  --基本全部实现

  1.制作手枪，冲锋枪，狙击枪（进阶选项）  --实现
  

（4）命中规则  --部分实现

 1.直接命中角色胶囊体  --实现
 
 2.精确命中模型，需要考虑性能（进阶选项）  --未实现
 


（5）怪物相关  --部分实现 

 1.制作具有一定AI的怪物；怪物可以寻路索敌，怪物会优先攻击NPC，被玩家攻击后吸引仇恨攻击玩家，仇恨消失继续攻击NPC --实现 (需要AIController、行为树、黑板、怪物角色协同完成)
 
 2.怪物能够近战攻击、远程攻击（进阶选项）  --实现
 
 3.制作阶段BOSS（进阶选项） --未实现
 

（6）其他规则 --部分实现

  1.小怪被击杀，随机掉落BUFF和枪械 --尝试实现但未实装，还有一些BUG没有解决
  
  2.BUFF道具系统（进阶选项） --实现 (开发了加速、加攻击力、加防御力、加血、加射速的多种BUFF，通过指定一个系数，数值参与计算时实时考虑该系数来实现)


*由于工程文件过大，仓库内容仅代表阶段性开发结果，目前还会有一些小问题，随着这个项目的持续完善，最终成果请参考微云链接



