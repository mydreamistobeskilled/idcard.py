# idcard. py
#This project is assigned to manage personal idcards
#We can add idcard to idcards. 
#We can remove idcard from idcards. 
#we can rewrite idcard. 
idcards=[]
def first_part():
    print('*'*66)
    print('请选择你的操作:')
    print('1.增加名片.')
    print('2.删除名片.')
    print('3.修改名片.')
    print('4.查询名片.')
    print('*'*66)

def addidcard():
    idcard={}
    idcard. setdefault('name',input('请输入你的姓名:'))
    idcard. setdefault('age',input('请输入你的年龄:'))
    idcard. setdefault('gender',input('请输入你的性别:'))
    idcard. setdefault('tel',input('请输入你的电话号码:'))
    idcards. append(idcard)

def delidcard():
   name=input('请输入要删除的姓名:')
   delstatus=False
   for idcard in idcards:
       if idcard. get('name')==name:
           delstatus=True
           del idcards
           break
           

while True:
    first_part()
    print('-'*66)
