import customtkinter 
customtkinter.set_appearance_mode('dark')
customtkinter.set_default_color_theme('dark-blue')
root=customtkinter.CTk()
root.geometry('500x350')
def logic():
    print('Test')
frame=customtkinter.CTkFrame(master=root)
frame.pack(pady=20, padx=60, fill='both', expand=True)
label=customtkinter.CTkLabel(master=frame, text='Logic System', font=('Arial', 24))
label.pack(pady=20, padx=10)
entry1=customtkinter.CTkEntry(master=frame, placeholder_text='Username')
entry1.pack(pady=12, padx=10)
entry2=customtkinter.CTkEntry(master=frame, placeholder_text='Password', show='*')
entry2.pack(pady=12, padx=10)
button=customtkinter.CTkButton(master=frame, text='Login', command=logic)
button.pack(pady=12, padx=10)
checkbox=customtkinter.CTkCheckBox(master=frame, text='Remember me')
checkbox.pack(pady=12, padx=10)
root.mainloop()
