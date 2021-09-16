from tkinter import *
import math

root = Tk()
root.title("simple calculator")

e = Entry(root, width=35, borderwidth=9)
e.grid(row=0, column=0, padx=10, pady=5,ipady=20, columnspan=5,sticky=W+E)


def button_click(number):
    display = e.get()
    e.delete(0, END)
    e.insert(0, str(display) + str(number))


def button_clear():
    e.delete(0, END)


def button_add():
    first_number = e.get()
    global Num
    global math
    math = "addition"
    Num = float(first_number)
    e.delete(0, END)


def button_sub():
    first_number = e.get()
    global Num
    global math
    math = "subtraction"
    Num = float(first_number)
    e.delete(0, END)


def button_mul():
    first_number = e.get()
    global Num
    global math
    math = "multiplication"
    Num = float(first_number)
    e.delete(0, END)


def button_div():
    first_number = e.get()
    global Num
    global math
    math = "divison"
    Num = float(first_number)
    e.delete(0, END)


def button_equal():
    second_number = e.get()
    e.delete(0, END)

    if math == "addition":
        e.insert(0,Num + float(second_number))

    if math == "subtraction":
        e.insert(0,Num - float(second_number))

    if math == "multiplication":
        e.insert(0,Num * float(second_number))

    if math == "divison":
        e.insert(0,Num / float(second_number))

    if math == "sq" :
        e.insert(0, Num*Num)

    if math == "sqrt" :
        e.insert(0, Num**0.5)

def button_sqrt():
    first_number = e.get()
    global Num
    global math
    math = "sqrt"
    Num = float(first_number)
    e.delete(0, END)


def button_sq():
    first_number = e.get()
    global Num
    global math
    math = "sq"
    Num = float(first_number)
    e.delete(0, END)

def button_backspace():
    length = len(e.get())
    e.delete(length-1,END)




# define buttons
button_1 = Button(root, text="1", padx=30, pady=40, command=lambda: button_click(1))
button_2 = Button(root, text="2", padx=30, pady=40, command=lambda: button_click(2))
button_3 = Button(root, text="3", padx=30, pady=40, command=lambda: button_click(3))
button_4 = Button(root, text="4", padx=30, pady=40, command=lambda: button_click(4))
button_5 = Button(root, text="5", padx=30, pady=40, command=lambda: button_click(5))
button_6 = Button(root, text="6", padx=30, pady=40, command=lambda: button_click(6))
button_7 = Button(root, text="7", padx=30, pady=40, command=lambda: button_click(7))
button_8 = Button(root, text="8", padx=30, pady=40, command=lambda: button_click(8))
button_9 = Button(root, text="9", padx=30, pady=40, command=lambda: button_click(9))
button_0 = Button(root, text="0", padx=30, pady=40, command=lambda: button_click(0))
button_add = Button(root, text="+", padx=30, pady=40, command=button_add)
button_sub = Button(root, text="-", padx=30, pady=40, command=button_sub)
button_div = Button(root, text="/", padx=30, pady=40, command=button_div)
button_mul = Button(root, text="*", padx=30, pady=40, command=button_mul)
button_equal = Button(root, text="=", padx=30, pady=40, command=button_equal)
button_clear = Button(root, text="clear", padx=30, pady=39, command=button_clear)
button_dot = Button(root, text=".", padx=31, pady=40, command=lambda: button_click("."))
button_sqrt= Button(root, text="^1/2", padx=20, pady=40,command=button_sqrt)
button_sq= Button(root, text="^2", padx=25, pady=40,command=button_sq)
button_backspace=Button(root, text="C", padx=25, pady=40,command=button_backspace)
# positioning

button_1.grid(row=3, column=0)
button_2.grid(row=3, column=1)
button_3.grid(row=3, column=2)

button_4.grid(row=2, column=0)
button_5.grid(row=2, column=1)
button_6.grid(row=2, column=2)

button_7.grid(row=1, column=0)
button_8.grid(row=1, column=1)
button_9.grid(row=1, column=2)

button_0.grid(row=4, column=1)
button_dot.grid(row=4, column=0)
button_add.grid(row=1, column=3)
button_sub.grid(row=2, column=3)
button_div.grid(row=3, column=3)
button_mul.grid(row=4, column=2)
button_equal.grid(row=4, column=3)
button_clear.grid(row=4, column=4,)
button_sqrt.grid(row=5,column=0)
button_sq.grid(row=5,column=1)
button_backspace.grid(row=5,column=2)




root.mainloop()
