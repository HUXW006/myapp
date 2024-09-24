#加法计算器-实时计算更新
#!/usr/bin/env python
from tkinter import *


class App(object):
    def __init__(self):
        self.top = Tk()
        self.top.title('加法计算-实时计算更新')
        self.res = StringVar(value='0.0')
        self.a = StringVar(value='0.0')
        self.b = StringVar(value='0.0')

        self.la = Label(self.top, text='加数A', width=8, fg='black', font=('Helvetica', 12))
        self.la.grid(row=0, column=0)
        self.na = Entry(self.top, width=10,  textvariable=self.a)
        self.na.bind('<KeyRelease>', self.addfun)
        self.na.grid(row=0, column=1)

        self.lb = Label(self.top, text='加数B', width=8, fg='black', font=('Helvetica', 12))
        self.lb.grid(row=0, column=2)
        self.nb = Entry(self.top, width=10,  textvariable=self.b)
        self.nb.bind('<KeyRelease>', self.addfun)
        self.nb.grid(row=0, column=3)

        self.lr = Label(self.top, text='结果', width=8, fg='black', font=('Helvetica', 12))
        self.lr.grid(row=1, column=0)
        self.nr = Entry(self.top, width=10, textvariable=self.res)
        self.nr.config(state='readonly')
        self.nr.grid(row=1, column=1)


    def addfun(self, env=None):
        self.res.set(str(float(self.na.get())+float(self.nb.get())))


def main():
    App()
    mainloop()


if __name__ == '__main__':
    main()
