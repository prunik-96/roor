from tkinter import *
import random



e = 1
GAME_WIDTN = 1400
GAME_HEIGHT = 700
SPACE_SIZE= 5
SPEED = 200
BACKGROUND_COLOR = "#007B58"
COLOR = "#007981"
COLOR2 = "#56955A"
COLOR3 = "#539295"
COLOR4 = "#FFA54F"
COLOR5 = "#C87667"
class o :
    def __init__(self):
        x = random.randint(0, (GAME_WIDTN / SPACE_SIZE)-1) * SPACE_SIZE
        y = random.randint(0, (GAME_HEIGHT / SPACE_SIZE)-1) * SPACE_SIZE
        
        self.coordinates = [x, y]
        
        self.oval = canvas.create_oval(x, y, x + SPACE_SIZE, y + SPACE_SIZE, fill = COLOR)
        
        o.e = 1
        
    def move(self):
        direction = random.choice(['UP', 'DOWN', 'LEFT', 'RIGHT'])
        if direction == "UP":
            self.coordinates[1] = self.coordinates[1] - 2
        if direction == "DOWN":
            self.coordinates[1] = self.coordinates[1] + 2
        if direction == "LEFT":
            self.coordinates[0] = self.coordinates[0] - 2
        if direction == "UP":
            self.coordinates[0] = self.coordinates[0] + 2
    
        canvas.delete(self.oval)
        self.oval = canvas.create_oval(self.coordinates[0], self.coordinates[1], self.coordinates[0] + SPACE_SIZE, self.coordinates[1] + SPACE_SIZE, fill = COLOR)
    

class s :

    def __init__(self):
        x = random.randint(0, (GAME_WIDTN / SPACE_SIZE)-1) * SPACE_SIZE
        y = random.randint(0, (GAME_HEIGHT / SPACE_SIZE)-1) * SPACE_SIZE
        
        s.e =+0.5
        
        print(s.e)
        
        s.coordinates = [x, y]
        
        canvas.create_oval(x, y, x + SPACE_SIZE, y + SPACE_SIZE, fill = COLOR2)
        
    
    

class d :
    def __init__(self):
        x = random.randint(0, (GAME_WIDTN / SPACE_SIZE)-1) * SPACE_SIZE
        y = random.randint(0, (GAME_HEIGHT / SPACE_SIZE)-1) * SPACE_SIZE
        
        m.coordinates = [x, y]
        
        canvas.create_oval(x, y, x + SPACE_SIZE, y + SPACE_SIZE, fill = COLOR4)

class r :
    def __init__(self):
        x = random.randint(0, (GAME_WIDTN / SPACE_SIZE)-1) * SPACE_SIZE
        y = random.randint(0, (GAME_HEIGHT / SPACE_SIZE)-1) * SPACE_SIZE
        
        r.coordinates = [x, y]
        
        canvas.create_oval(x, y, x + SPACE_SIZE, y + SPACE_SIZE, fill = COLOR5)

class m :
    def __init__(self):
        x = random.randint(0, (GAME_WIDTN / SPACE_SIZE)-1) * SPACE_SIZE
        y = random.randint(0, (GAME_HEIGHT / SPACE_SIZE)-1) * SPACE_SIZE
        
        m.coordinates = [x, y]
        
        canvas.create_oval(x, y, x + SPACE_SIZE, y + SPACE_SIZE, fill = COLOR4)

class ww :
    def __init__(self):
        x = random.randint(0, (GAME_WIDTN/SPACE_SIZE)-1) * SPACE_SIZE
        y = random.randint(0, (GAME_HEIGHT/SPACE_SIZE)-1) * SPACE_SIZE
        
        self.coordinates =[x, y]
        
        canvas.create_oval(x, y, x + SPACE_SIZE, y + SPACE_SIZE,  fill = COLOR3)
        
    
window = Tk()
window.title("roor")
window.resizable(False, False)

canvas = Canvas(window, bg = BACKGROUND_COLOR, height = GAME_HEIGHT, width = GAME_WIDTN)
canvas.pack()

window.update()

window_width = window.winfo_width()
window_height = window.winfo_height()
screen_width = window.winfo_screenwidth()
screen_height = window.winfo_screenheight()

x = int((screen_width/2) - (window_width/2))
y = int((screen_height/2) - (window_height/2))

window.geometry(f"{window_width}x{window_height}+{x}+{y}")


# O = o()
ovals = []
for x in range(0, 999):
    ovals.append(o())

def next_turn(ovals) :        
    for o in ovals:
        o.move()
    window.after(50, next_turn, ovals)

next_turn(ovals)

# S = s()
ovals = []
for x in range(0, 499):
    ovals.append(s())

def next_turn(ovals) :        
    for s in ovals:
        s.move()
    window.after(50, next_turn, ovals)

# WW = ww()
ovals = []
for x in range(0, 249):
    ovals.append(ww())
    
# D = d()
ovals = []
for x in range(0, 1):
    ovals.append(d())
    
    
# M = m()
ovals = []
for x in range(0, 499):
    ovals.append(m())
    
    
# r = r()
ovals = []
for x in range(0, 119):
    ovals.append(r())

        

window.mainloop()