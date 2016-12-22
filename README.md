# YTSendGiftDemo
# 功能：模拟直播间送礼物，连击倒计时为15s，超过15s则连击失效。
# 核心实现：
# 1、收到礼物后，创建任务，并加入队列（判断是否有缓存）
# 2、将任务加入缓存operationCache中，并存储该任务对应的礼物信息于userGiftInfos中（缓存的key由用户名和礼物名称拼接而成）。
# 3、动画模块是使用回调块实现(递归)。
