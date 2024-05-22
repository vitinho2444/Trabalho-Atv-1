import tkinter as tk

def double_number():
    input_num = int(entry.get())
    result = input_num * 2
    label_result.config(text=f'O dobro do número é: {result}')

# Create the main window
root = tk.Tk()
root.title("Dobro do número")

# Create the input entry widget
entry = tk.Entry(root)
entry.pack()

# Create a button to trigger the function
button = tk.Button(root, text="Calcular Dobro", command=double_number)
button.pack()

# Create a label to show the result
label_result = tk.Label(root, text="")
label_result.pack()

# Start the main loop
root.mainloop()
