# LiDAR Device 🤖
A datasheet and a set of code dedicated to the development of a LiDAR device used to scan hallways up to 4m wide. This project employs a Texas Instruments MSP432E401Y microcontroller and a ToF sensor. Programming was done in C for backend structuring and Python for data visualization. 

All information, including programming workflows and circuit schematics, is provided in the datasheet.

---

The image below depicts the circuit employed in the finalized edition of the device. It tactically makes use of a shoebox to steadily hold a ToF sensor mounted on a stepper motor. The code flashed onto the microcontroller instructs the motor to spin in a certain direction while the ToF sensor captures distance measurements at various x-axis intervals. After the completion of an _n_ number of sets, a 3D image is compiled via Open3D through Python. 

![image](https://github.com/user-attachments/assets/179a504b-3e78-457b-ac41-df21784af3b6)

Below is an example of a hallway scan. It is important to note that specific factors like light bulbs and building structure can cause the receptor of the ToF sensor to produce false measurements, hence explaining a few distortions that are visible. 

![image](https://github.com/user-attachments/assets/59fae58f-f74c-445e-a24d-06389ade1a43)
