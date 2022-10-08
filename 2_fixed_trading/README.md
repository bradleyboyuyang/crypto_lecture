#### 一些注意事项

**关于手续费**

手续费的计算存在不精确，比如滑点应该加在价格上，手续费则扣在现金上。

注：binance普通用户币币现货手续费为0.1%（无论挂单或吃单），5周年庆目前BTC/USDT现货交易免手续费。

**超参数**

1. 定投的资金量，可以直接修改代码回测。
2. 定投频率，更改定投频率则需要从高频的数据resample到不同频率，再跑测试代码。data文件夹提供有12h和1D的数据，可以自行降频到3、5、7天查看效果。
3. 回测时间


**回测时间的选取，以BTC为例**
- 牛市回测：2017-01-01到2017-12-31，并未跑过本身涨幅
- 熊市回测：2018-01-01到2018-12-31，少亏很多
- 长期回测：2006至今，稳赚不赔（只要长期看好向上）
- 最坏情况：牛市顶点开始定投，BTC从2013-12-04开始，或者EOSUSD从2018-01-13到2018-04-26
- BTC完整的微笑曲线：2017-12-17到2018-05-05，比特币腰斩，定投不亏
- 观测定投微笑曲线如何降低平均持币成本：BTCUSD，2013-12-04到2015-12-31，牛市顶点定投，持币成本最后还会低于收盘价

