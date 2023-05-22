# label-the-IP-address

# Create a frame for the IP address label and entry field
ip_frame = tk.Frame(main_tab)
ip_frame.pack(side=tk.TOP, pady=20)


# Create label and entry field for IP address
ip_label = tk.Label(ip_frame, text="Enter the IP address to scan:")
ip_label.pack(side=tk.TOP, padx=10, pady=10)

ip_entry = tk.Entry(ip_frame)
ip_entry.pack(side=tk.TOP, padx=10, pady=10)

# Create label to display the port scan and attack detection results
scan_result_label = tk.Label(main_tab, text="")
scan_result_label.pack()

# Create the buttons and pack them side by side
scan_button = tk.Button(main_tab, text="Scan Ports", command=scan_ports)
scan_button.pack(side=tk.TOP, padx=(20, 5), pady=5)
