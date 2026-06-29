from tkinter import *

root = Tk()
root.title("Thiranex Assignment")
root.geometry("430x750")
root.configure(bg="#f2f5fb")

card = Frame(root, bg="white", bd=1, relief="solid")
card.place(x=20, y=20, width=390, height=520)

Label(card, text="3",
      bg="#eaf2ff",
      fg="#2563eb",
      font=("Arial", 18, "bold"),
      width=3,
      height=2).place(x=20, y=20)

Label(card,
      text="AVAILABLE",
      bg="#eef4ff",
      fg="#2563eb",
      font=("Arial", 10, "bold"),
      padx=10,
      pady=4).place(x=290, y=25)

Label(card,
      text="Due Date: 22 Jun 2026",
      bg="white",
      fg="gray30",
      font=("Arial", 11)).place(x=20, y=90)

Label(card,
      text="Overdue by 6 Days",
      bg="#ffe5e5",
      fg="#c62828",
      font=("Arial", 10, "