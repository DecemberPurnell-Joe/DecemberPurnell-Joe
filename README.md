import tkinter as tk

def draw_godzilla(canvas):
    # Body
    canvas.create_rectangle(200, 140, 400, 440, fill='#5e5e5e', outline='black', width=2)
    # Head
    canvas.create_rectangle(260, 20, 340, 140, fill='#5e5e5e', outline='black', width=2)
    # Tail
    canvas.create_rectangle(100, 220, 130, 440, fill='#5e5e5e', outline='black', width=2)
    # Legs
    canvas.create_rectangle(200, 440, 260, 580, fill='#5e5e5e', outline='black', width=2)
    canvas.create_rectangle(340, 440, 400, 580, fill='#5e5e5e', outline='black', width=2)
    # Arms
    canvas.create_rectangle(160, 240, 200, 340, fill='#5e5e5e', outline='black', width=2)
    canvas.create_rectangle(400, 240, 440, 340, fill='#5e5e5e', outline='black', width=2)
    # Eyes
    canvas.create_oval(280, 60, 290, 70, fill='white', outline='black', width=1)
    canvas.create_oval(310, 60, 320, 70, fill='white', outline='black', width=1)
    # Spikes
    canvas.create_polygon(220, 80, 260, 120, 220, 140, fill='#4d4d4d', outline='black', width=2)
    canvas.create_polygon(240, 120, 280, 160, 240, 180, fill='#4d4d4d', outline='black', width=2)
    canvas.create_polygon(260, 160, 300, 200, 260, 220, fill='#4d4d4d', outline='black', width=2)
    canvas.create_polygon(280, 200, 320, 240, 280, 260, fill='#4d4d4d', outline='black', width=2)

# Initialize the main window
root = tk.Tk()
root.title("Godzilla Drawing")

# Create a canvas widget
canvas = tk.Canvas(root, width=600, height=600, bg='#e0e0e0')
canvas.pack()

# Draw Godzilla on the canvas
draw_godzilla(canvas)

# Run the application
root.mainloop()
