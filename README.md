from tkinter import *

root = Tk()
root.title("Website UI Redesign")
root.geometry("420x750")
root.configure(bg="#f3f6fb")

# Card
card = Frame(root, bg="white", bd=1, relief="solid")
card.place(x=20, y=30, width=380, height=650)

# Task Number
Label(card, text="2", bg="#eaf2ff", fg="#2d6cdf",
      font=("Arial", 18, "bold"), width=3, height=1).place(x=20, y=20)

# Available Badge
Label(card, text="AVAILABLE", bg="#eaf8ff", fg="#2d6cdf",
      font=("Arial", 10, "bold"), padx=10, pady=5).place(x=260, y=20)

# Due Date
Label(card, text="Due Date: 15 Jun 2026",
      bg="white", fg="gray30",
      font=("Arial", 11)).place(x=20, y=90)

# Overdue Badge
Label(card, text="Overdue by 13 Days",
      bg="#ffd9d9", fg="#b00020",
      font=("Arial", 10, "bold"),
      padx=10, pady=5).place(x=210, y=85)

# Title
Label(card, text="Website UI Redesign",
      bg="white", fg="black",
      font=("Arial", 18, "bold")).place(x=20, y=140)

# Description
desc = "Redesign the user interface of an existing website to improve usability."
Label(card, text=desc, bg="white", fg="gray25",
      font=("Arial", 11), wraplength=330,
      justify="left").place(x=20, y=180)

# Key Features
Label(card, text="Key Features:",
      bg="white", fg="#2563eb",
      font=("Arial", 13, "bold")).place(x=20, y=250)

features = [
    "Perform heuristic evaluation to identify usability issues",
    "Create mood boards and style guides",
    "Design high-fidelity mockups",
    "Ensure responsive layouts for desktop and mobile"
]

y = 285
for feature in features:
    Label(card,
          text="• " + feature,
          bg="white",
          fg="black",
          font=("Arial", 11),
          wraplength=320,
          justify="left").place(x=30, y=y)
    y += 55

# Expected Outcome
Label(card,
      text="Expected Outcome:",
      bg="white",
      fg="green",
      font=("Arial", 13, "bold")).place(x=20, y=510)

outcome = "Gain experience in visual hierarchy, layout design, and responsive design."

Label(card,
      text=outcome,
      bg="white",
      fg="gray25",
      font=("Arial", 11),
      wraplength=330,
      justify="left").place(x=20, y=545)

root.mainloop()