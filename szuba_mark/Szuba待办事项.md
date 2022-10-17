# Szuba Todo List
### Start Date  :*05/18/2022*
1. ~~**帧数调整**的优化~~
2. ~~**已标记与未标记**的文件做区分~~
3. **进度条显示**关键帧(start,end,markd)
4. ~~非所在帧显示优化~~(temp)
5. landmark的优化(**主动脉**无法用点表达)
6. ~~**播放与暂停**键(check box可以选取是由**起止帧或者全段播放**)~~
7. Draw **line** by marks
8. ~~修复在未导入dicom时点击MINI、保存时崩溃的bug~~



### Date  :*05/20/2022*
1. ~~**Chosen Button**~~
2. ~~**Loaded logic选中的文件自动标记了**~~
3. Config文件的扩充：(size,width,fill...etc)
4. ~~loaded显示不完全~~
5. ~~滚轮键冲突~~


### Date  :*05/21/2022*
1. ~~savemarks后 修改标点table未正常显示~~
2. ~~非所在帧的点的删除~~

### Date  :*06/12/2022*
1. ~~szuba对avi格式的兼容~~
2. ~~播放卡顿问题(Plan b)~~
3. 独立出dicom player

### Date :06/25/2022

1. ~~每个病人ID对应的dicom之间的区分（Instance Number）~~
2. 读取非视频dicom（单帧）时：File F:\bawk\szuba0626b\szuba.py:449 in <module>
       rownum = values[kSTUDYTABLE][0]
3. 对各种形式的dicom的兼容
4. cfg修改后的bug
5. szuba对ID的搜索的记忆功能

### Date :06/28/2022

* ~~读取卡顿问题的记录（2min 1500）（加载后无卡顿）~~

* 通过avi寻找对应dicom的脚本
* ~~打开txt 表格呈现对应文档~~
* 通过dpath直接生成对应标记帧数的png（无损）Or 自己选择的帧数
* dpath2img 输入name 选出所有相应name帧数（例如左心室）
* 