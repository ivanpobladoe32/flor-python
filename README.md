import turtle

ventana = turtle.Screen()
ventana.bgcolor("white")

flor = turtle.Turtle()
flor.shape("turtle")
flor.speed(10)

def dibujar_petalo():
    flor.color("red")
    flor.circle(100, 60)  # Dibuja un arco de 60 grados con un radio de 100
    flor.left(120)         # Gira a la izquierda 120 grados
    flor.circle(100, 60)  # Dibuja el otro arco
    flor.left(120)

for _ in range(6):  # Dibujará 6 pétalos
    dibujar_petalo()
    flor.left(60)  # Gira 60 grados para colocar el siguiente pétalo

flor.color("green")
flor.right(90)
flor.forward(250)

flor.hideturtle()
ventana.mainloop()
