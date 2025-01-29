# Digital-Clock-Using-in-Python

**Digital Clock**

This project is a digital clock application developed using Python and Tkinter. The clock displays the current time in hours, minutes, seconds, and AM/PM format with a clean and stylish design.

**Features**

Real-Time Display: Shows the current time updated every second.

Stylish Interface: Customizable font, colors, and design elements.

AM/PM Format: Displays the time in HH:MM:SS AM/PM format for clarity.

Responsive Layout: The clock adjusts to fill the window size.


**Full Code**

Here is the complete code for the digital clock:
import tkinter as tk
from time import strftime

#Create the main window
root = tk.Tk()
root.title("Digital Clock")

#Define the clock label with improved styling
clock_label = tk.Label(root, 
                       font=("Helvetica", 60), 
                       bg="black", 
                       fg="cyan", 
                       bd=30, 
                       relief="sunken")
clock_label.pack(anchor="center", fill="both", expand=True)

#Function to update the time
def update_time():
    current_time = strftime("%H:%M:%S %p")  # Added AM/PM format
    clock_label.config(text=current_time)
    clock_label.after(1000, update_time)

#Initialize the clock
update_time()

#Run the main loop
root.mainloop()


**📌 Connect With Me**

If you’re interested in exploring how data visualization can transform your business operations, feel free to connect with me!

📧 deepakkumarsingh7774@gmail.com

🔗 https://www.linkedin.com/in/deepakkumar7774

🌐 https://github.com/Deepakkumar7774/-Digital-Clock-Using-in-Python

