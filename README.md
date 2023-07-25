import random

print("欢迎来到石头、剪刀、布游戏！")
print("请选择：1. 石头 2.剪刀 3.布")

# 用户输入
user_choice = int(input())

# 电脑随机选择
computer_choice = random.randint(1, 3)

# 根据选择输出结果
if user_choice == 1:
    if computer_choice == 1:
        print("平局！")
    elif computer_choice == 2:
        print("你赢了！")
    else:
        print("电脑赢了！")
elif user_choice == 2:
    if computer_choice == 1:
        print("电脑赢了！")
    elif computer_choice == 2:
        print("平局！")
    else:
        print("你赢了！")
elif user_choice == 3:
    if computer_choice == 1:
        print("你赢了！")
    elif computer_choice == 2:
        print("电脑赢了！")
    else:
        print("平局！")
else:
    print("输入错误，请重新输入！")
