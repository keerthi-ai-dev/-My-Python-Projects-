from tkinter import *

root = Tk()
root.title("Usability Testing & Analysis")
root.geometry("430x750")
root.configure(bg="#f2f5fb")

card = Frame(root, bg="white", bd=1, relief="solid")
card.place(x=20, y=20, width=390, height=620)

# Number Box
Label(card,
      text="4",
      bg="#eef4ff",
      fg="#2563eb",
      font=("Arial", 18, "bold"),
      width=3,
      height=2).place(x=20, y=20)

# Available Badge
Label(card,
      text="AVAILABLE",
      bg="#eef4ff",
      fg="#2563eb",
      font=("Arial", 10, "bold"),
      padx=12,
      pady=5).place(x=285, y=25)

# Due Date
Label(card,
      text="📅 Due Date: 29 Jun 2026",
      bg="white",
      fg="#555555",
      font=("Arial", 11)).place(x=20, y=90)

# Days Left Badge
Label(card,
      text="1 Days Left",
      bg="#d7f8df",
      fg="#138a4a",
      font=("Arial", 10, "bold"),
      padx=10,
      pady=5).place(x=300, y=85)

# Divider
Frame(card, bg="#e6e6e6", height=1, width=340).place(x=20, y=130)

# Title
Label(card,
      text="Usability Testing & Analysis",
      bg="white",
      fg="#111827",
      font=("Arial", 18, "bold"),