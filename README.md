Binary Clock & Calendar using VGA (FPGA - Verilog)

Overview

A real-time digital clock and calendar system implemented on FPGA, displaying time visually using binary representation via VGA output. This project blends digital logic design with graphical signal generation.


 Key Features

* Binary representation of time (Hours, Minutes, Seconds)
* Calendar integration (Date/Month/Year)
* VGA display output (real-time visualization)
* AM/PM mode control
* Manual adjustment using switches/buttons
* Modular Verilog design



 System Architecture

* **Clock Divider** → Generates required timing signals
* **Binary Clock Module** → Maintains time logic
* **Calendar Logic** → Tracks date transitions
* **VGA Controller** → Generates sync signals
* **Pixel Generator** → Controls display output
* **ROM Module** → Stores digit patterns



 Project Structure


binary-clock-and-calender-vga/
│
├── src/
│   ├── design_top.v
│   ├── new_binary_clock.v
│   ├── pixel_gen.v
│   ├── vga_controller.v
│   ├── clock_digit_rom.v
│   ├── top_clk_cal.v
│
├── constraints/
│   └── const_vga_clk_cal.xdc
│
├── README.md
├── .gitignore

 Hardware Requirements

* Basys 3 FPGA Board
* VGA Monitor
* Connecting cables



 How to Run

1. Open Xilinx Vivado
2. Create a new RTL project
3. Add all Verilog files from `src/`
4. Add constraint file from `constraints/`
5. Run synthesis → implementation → generate bitstream
6. Program FPGA board
7. Connect VGA → observe output



Output

<img width="897" height="504" alt="image" src="https://github.com/user-attachments/assets/f02b744d-7ec2-494f-9930-d0fa529192a5" />




 Future Enhancements

* Alarm functionality
* Color customization
* 12/24-hour toggle
* GUI-style interface
* Touch/button UI improvements



 Learning Outcomes

* Digital system design using Verilog
* VGA signal generation
* Timing and synchronization
* FPGA-based real-time systems


