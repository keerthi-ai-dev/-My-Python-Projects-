import tkinter as tk

root = tk.Tk()
root.title("Mobile App Wireframe")
root.geometry("300x600")

tk.Label(root, text="Login", font=("Arial", 18, "bold")).pack(pady=20)

tk.Label(root, text="Username").pack()
tk.Entry(root).pack(pady=5)

tk.Label(root, text="Password").pack()
tk.Entry(root, show="*").pack(pady=5)

tk.Button(root, text="Login", width=20).pack(pady=20)

tk.Label(root, text="Forgot Password?", fg="blue").pack()

root.mainloop()