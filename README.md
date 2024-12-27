# **Network Anomaly Detection Using Machine Learning**

### **Overview**
This project implements a machine learning-based network anomaly detection system capable of identifying irregularities in network traffic, such as SYN flood attacks and other anomalies. The system uses a virtual network environment for simulation and captures data with Wireshark. It employs the Isolation Forest algorithm for anomaly detection and integrates the results into a Flask-based web application for real-time user interaction.

---

### **Features**
- **Virtual Network Environment**: Simulates real-world network traffic with both normal and anomalous patterns.  
- **Anomaly Detection**: Utilizes the Isolation Forest algorithm to identify SYN flood attacks and other anomalies.  
- **Web Application**: Flask-based interface for uploading network traffic files and visualizing results.  
- **Real-Time Feedback**: Provides immediate insights into network health through anomaly analysis.  

---

### **Technologies Used**
- **Programming Language**: Python  
- **Machine Learning Libraries**: Scikit-learn, Pandas, NumPy, Matplotlib  
- **Networking Tools**: Wireshark, hping3, Nmap  
- **Web Framework**: Flask  

---

### **Usage**
1. **Data Capture**:
   - Simulate normal traffic using `curl` and anomalous traffic using tools like `hping3` for SYN flood attacks.
   - Use Wireshark to capture network traffic and export it as `.csv` files.

2. **Run Anomaly Detection**:
   - Upload the `.csv` file through the Flask web interface.
   - View anomalies and results directly in the browser.

3. **Command Example**:  
   ```bash
   hping3 -S --flood -p 80 server-ip
   ```

---

### **Results**
- **Machine Learning Model**: The Isolation Forest algorithm identifies anomalies with precision.  
- **Anomaly Visualizations**: Results are displayed via a user-friendly web interface, highlighting anomalies in uploaded traffic data.

---

### **Future Enhancements**
1. **Real-Time Detection**: Implement real-time processing for live network data streams.  
2. **Advanced ML Models**: Explore deep learning models to improve accuracy.  
3. **Explainability**: Add features to explain detected anomalies for better understanding.  
4. **Scalability**: Adapt for multi-tenant and cloud-based deployments.  

---

### **Contributing**
Contributions are welcome! Follow these steps:  
1. Fork the repository.  
2. Create a new branch (`feature/your-feature`).  
3. Commit changes and push to the branch.  
4. Submit a pull request.  

---

### **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to explore, contribute, and use this project to enhance network security!
