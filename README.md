# panda
import turtle
import math

screen = turtle.Screen()
screen.setup(width = 700, height = 500)
screen.bgcolor("light blue")

pen = turtle.Turtle()
pen.speed(0)
pen.hideturtle()

def draw_circle(colour, x, y, radius):
  pen.penup()
  pen.goto(x,y)
  pen.pendown()
  pen.color(colour)
  pen.begin_fill()
  pen.circle(radius)
  pen.end_fill()
  
# ears
draw_circle("black", -60, 90, 30)
draw_circle("black", 60, 90, 30)
# body
draw_circle("white", 0, 0, 75)
# eyes
draw_circle("black", -40, 50, 30)
draw_circle("black", 40, 50, 30)
