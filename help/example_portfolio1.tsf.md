# selfportfliooptimizer
*����:* type

**˵��**

>  ����Ż�����չ ,�޸�init����������չԼ��;
   �����Ĭ������1\. �����Ļ�׼Ϊָ������(���Բ�������getydata����) 2\. ��׼ָ���ɷ��ڸ���������\_infodata�п����ҵ�
   3\.������\_infdata����˵���е��ֶ�


***
*����:* tsportfoliooptimizer;
## ��Ա����
|����|������|����|˵��|�Ƿ�̬����
|--|--|--|--|--
|_infdata|public|array| ��Ϣ, Լ�������ȶ������л������<br>                           ��ά��������ֶ�<br>                           "����" : ֤ȯ����<br>                           "����" : ֤ȯ����<br>                           "����(%)" : ʵ�ʱ���<br>                           "�����½�(%)" : ���Ʊ����½�<br>                           "�����Ͻ�(%)" : ���Ʊ����Ͻ�<br>                           "��ҵ����",  :��ҵ����<br>                           �����ֶ���Լ��ʱʹ��<br>                           "��ͨ��ֵ"<br>                           "����ֵ"	,<br>                           "���ʲ�",<br>                           "�ܹɱ�",<br>                           "EP",<br>                           "BP",<br>                           "�ۺ�����"|



## ��������
|������|��������|������|�Ƿ�̬����|virtual
|--|--|--|--|--
|getinfodata|0|public|0|
|init|0|public|0|

**����**<br>
[selfportfliooptimizer����](../code/example_portfolio1.tsf)<br>
**�������** <br>
![����ת��](../img/zhgzyh001.jpg)

��ϸ��ٷ���\-
```
obj := new   selfportfliooptimizer();
obj.FIndexID := "SH000300" ;//���û�׼ָ��
Obj.FBegT:=20160107T; //���ٿ�ʼʱ��  
Obj.FEndT:=20170107T; //���ٽ�ֹʱ��
Obj.FObjType:=1;   //�����������
Obj.FConType:=0;  // ���÷�����Լ�� �������
obj.FThresholdUpper:=15;  //���÷�����Լ���Ͻ�
obj.init(); //����Լ��
Ret:=obj.PortfolioOptimize();
return  array(
              "�Ż���Ϣ":Ret,
              "�Ż������":obj.GetPortfolioData(),
              "�Ż�����":obj.GetReturnandRisk()
              );
```
## getinfodata
*����:* function
*������:* public


**˵��**

>  �޸Ĵ˺����� \_infdata ��ֵ;


**����:getinfodata();**

## init
*����:* function
*������:* public


**˵��**

>  �˺�����������Լ��
	  1\. �������½�
	  2\. ��׼��ҵռ��
	  3\. ��ֵ��׼ռ��
	  4\. bp��׼ռ��


**����:init();**


***
