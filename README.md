# 四柱_八字_bazi_干支排盘
##简介
This is my first taste to make a Bazi row that can use anydate(include BC and AD).  This work is not easy for me, but has much fun.
初次尝试写一个简要的八字排盘程序，可以不限公元前后，对日期进行干支排盘计算。
查阅网上的计算方法，包括口诀法、查表法等，目前已经实现年月日时干支的计算，但仍有较多缺陷。
1.  不能计算二十四节气（重大缺陷）
2.  程序中引用了一个别人写的公历和农历转换，但是经测试不是很准确，且范围有限（1900-2049）
3.  可转换公历的程序段在最后的注释中，需要的可以使用
4.  主程序需要知道某一日期的公历和农历方可计算
6.  需要知道十二个时辰的序号
##计算方法简介
1. 年柱：公元4年为甲子年，天干10进制，地支12进制，用取余计算干支
2. 月柱：计算完年干，取年干序号，用奇数序列；月支用正月建寅
3. 日柱：用年数表+月数表法，取80年作进制取余
4. 时柱：方法同月术，用序号及奇数序列；日支用子时建日
##计划
1. 希望能加入节气计算
2. 希望能按历法校正部分时间的错误
3. 远期加入解盘计算的数据
