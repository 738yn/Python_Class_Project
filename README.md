import turtle

# 创建一个Turtle窗口
screen = turtle.Screen()
screen.title("五角星图案")

# 创建一个Turtle对象
pen = turtle.Turtle()

# 设置画笔速度
pen.speed(3)

# 五角星的边长
side_length = 100

# 绘制五角星
for _ in range(5):
    pen.forward(side_length)  # 向前移动
    pen.right(144)            # 向右转144度（360度 / 5 * 2 = 144度，因为五角星的内角是36度，外角是144度）

# 完成绘制后隐藏画笔并显示窗口
pen.hideturtle()
turtle.done()
