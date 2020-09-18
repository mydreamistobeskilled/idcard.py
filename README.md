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
def namere():
    idcard={}
    idcard. setdefault('name',input('请输入你的姓名:'))
    return idcard

def agere():
    idcard={}
    idcard. setdefault('age',input('请输入你的年龄:'))
    return idcard

def genderre():
    idcard={}
    idcard. setdefault('gender',input('请输入你的性别:'))
    return idcard

def telre():
    idcard={}
    idcard. setdefault('tel',input('请输入你的电话号码:'))
    return idcard

def addidcard():
    idcard={}
    idcard. update(nanere())
    idcard. update(agere())
    idcard. update(genderre())
    idcard. update(telre())
    idcards. append(idcard)

def delidcard():
    name=input('请输入要删除的姓名:')
    delstatus=False
    for idcard in idcards:
        if idcard. get('name')==name:
            delstatus=True
            idcards. remove(idcard)
            break
    if delstatus:
        print('删除成功!')
    else:
        print('没有此人!')

def rewtidcard():
    name=input("请输入你要修改的姓名:")
    rewtstatus=False
    for idcard in idcards:
        if idcard. get('name')==name:
            rewtstatus=True
            num=input('请输入要修改的内容:1.姓名2.年龄3.性别4.电话.')
            if num=='1':
                idcard. update(namere())
            elif num=='2':
                idcard. updtae(agere())
            elif num=='3':
                idcard. update(genderre())
            elif num=='4':
                idcatd. update(telte())
            else:
                print('没有此修改项!')
            break
    if rewtstatus:
        print('修改成功!')
    else:
        print("没有此人!")

def checkidcard():
    name=input('请输入要查询的姓名:')
    for idcard in idcards:
        if idcard. get('name')==name or name=='all'
            print(idcard)


while True:
    first_part()
    print('-'*66)
