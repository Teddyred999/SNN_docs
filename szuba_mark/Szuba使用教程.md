# Szuba标记软件使用流程

## * 程序界面
![image](https://user-images.githubusercontent.com/91119822/171568979-d81b0aa1-e83e-42ff-ae6e-e04071d3f040.png)

## 软件使用流程

1. 文件导入流程

    1. 通过Browse按钮选取Dicom文件所在文件夹

    2. 点击Select按钮后，单击选取所需要标记的文件

    3. 等待导入完成后会在右侧图框显示整个Dicom的图像

        ![image](https://user-images.githubusercontent.com/91119822/171569971-85eada2a-9522-4473-90f7-9fb79a6ace49.png)

2. 标记流程
   
    1. 使用Frame# 栏的滑块或者键盘左右方向键调整呈现的帧数(短按调1帧，长按连续跳帧)

    2. 选取到某合适帧数时，需要标记可以先选取左侧对应标记按钮(以左心室为例，单击左心室时，按钮变成白色证明左心室A被选中)
    3. 左心室A按钮为白色时，可以在右侧超声图中标记相应位置(需要删除时只需点击删除按钮，在对应已标记的点上选取即可)
   
         ![image](https://user-images.githubusercontent.com/91119822/171571867-13c566ed-b3e0-4663-a5e5-d76bd2a179dd.png)

         ![image](https://user-images.githubusercontent.com/91119822/171573072-1379611c-ae99-4b36-97b9-12de3d17efe3.png)

    4. 在按照要求在几个心动周期内标记完成后，点击右下加Save Marks按钮即可将数据保存，接下来可以重复该流程标记下一个Dicom文件
   
    5. 在下次再导入已保存的Dicom数据时，之前保存的数据会显示在图中


## 关于程序的一些特殊说明

1. 在程序的左上角的表格内，标记栏内，有四种文件的不同状态：
   
   "saved"是当前文件的数据已被保存 
   
   "loaded"是该文件已被保存过   
   
   "mod"时该文件正在被修改、操作 
   
   "none"是指该文件未被操作

    ![image](https://user-images.githubusercontent.com/91119822/171574777-e39b42f8-e1be-4907-9d79-7ef3c80097c5.png)

2. 关于左下角信息的说明
   
    No.Marks与No.Points分别是已标记的部位数与已标记的标记点个数

    Strat Frame与End Frame分别是该Dicom数据的起始帧(起始帧为医生控制，若未对起始帧进行操作，则自动输入为Dicom文件的最大与最小帧数)

    ![image](https://user-images.githubusercontent.com/91119822/171575782-3e9910ac-9a44-4ade-87c7-ecae1850effc.png)

3. 关于右下角的按钮说明
    
    右下角的Strat Frame与End Frame与上面对应，医生可以通过标记合适的起止帧来选取最优的片段

    ![image](https://user-images.githubusercontent.com/91119822/171575870-ef211180-909b-4292-b8d1-6c7f34b51829.png)

   图中FR的按钮可以通过输入帧率来调整Dicom的播放速度，上限为20

   右侧的Play Clip Only可以只挑选所选定的起始帧进行播放(不勾选时默认播放完整文件)

   play按钮可以对Dicom文件进行播放和暂停操作(数字键0也可以达成相同效果)


4. 关于左下角缩略图的说明(Dicom MINI)Click able

    ![image](https://user-images.githubusercontent.com/91119822/171660157-0ed97fa1-1286-4fc7-95b2-c8d2900546c8.png)

    标记Dicom后，会自动生成左下侧标记所在帧缩略图(最多4张)，当其被点击时，右侧显示框内会跳到该标记所在帧
   
    






