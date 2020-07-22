from tkinter import *
from PIL import ImageTk, Image

screen = Tk()
screen.geometry("300x450")
screen.configure(bg='powderblue')

screen.title("Loan Interest Software")


def interest_calculator():
    loan_interest = (float(property_price.get())*float(spinboxvar.get())*float(interest_rate.get()))/100
    total_payment = float(property_price.get())+loan_interest
    result.set(f'Your total payment with interest is AED {total_payment}')


Label(text="", bg='powderblue').pack()
Label(text="Loan Interest Calculator", bg='gold').pack()

Label(text="", bg='powderblue').pack()
Label(text="Enter Property Price (AED)", bg='powderblue').pack()
property_price = Entry(screen)
property_price.pack()

Label(text="", bg='powderblue').pack()
Label(text="Enter Loan Period (Years)", bg='powderblue').pack()
spinboxvar = StringVar(screen)
SpinBox1 = Spinbox(screen,width=18, from_=1, to=30, increment=1, textvariable=spinboxvar)
SpinBox1.pack()

Label(text="", bg='powderblue').pack()
Label(text="Enter Interest Rate (%)", bg='powderblue').pack()
interest_rate = Entry(screen)
interest_rate.pack()

Label(text="", bg='powderblue').pack()
Button(text="Calculate", command=interest_calculator, bg='RosyBrown1').pack()

Label(text="", bg='powderblue').pack()
result = IntVar()
Label(text="", textvariable=result).pack()


def show_image():

    canvas = Canvas(screen, width=150, height=150, bg='powderblue', highlightthickness=0)
    canvas.pack()

    img = Image.open("5a46848ab4df7b9cbf90d7dd73c4a855-simple-house-black-silhouette-by-vexels.png")
    img = img.resize((150, 150), Image.ANTIALIAS)
    img = ImageTk.PhotoImage(img)
    canvas.create_image(78, 150, anchor=S, image=img)
    screen.mainloop()


if __name__ == '__main__':
    show_image()
