# tugas-d2-sekuro18-18225054

# Destroyer II - ROS2 Project

## Identitas

* Nama: Farel Athaya Yudha
* NIM: 18225054
* Kelompok: SEKURO 18

---

# Deskripsi Program

Program ini merupakan implementasi dasar sistem pergerakan robot Destroyer II menggunakan ROS2. Sistem memiliki dua mode:

 Autonomous Mode (gerakan random)
 Driver Mode (input keyboard)

Program menggunakan konsep inverse kinematics sederhana untuk menentukan arah gerak robot berdasarkan data Twist.



# Diagram Program


auto_mode_destroyer ----> 
                          \
                           > check_move_destroyer ---> /power_destroyer ---> move_destroyer
                          /
drive_mode_destroyer --->

check_move_destroyer ---> /move_type ---> move_destroyer




# Dependencies

 ROS2 (Humble/Foxy)
 C++
 colcon
 geometry_msgs
  std_msgs



# Cara Menjalankan

Build:

bash
colcon build


Source:

bash
source install/setup.bash


Run node:

bash
ros2 run destroyer auto_mode_destroyer


bash
ros2 run destroyer drive_mode_destroyer


bash
ros2 run destroyer check_move_destroyer


bash
ros2 run destroyer move_destroyer


