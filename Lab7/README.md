<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab7">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab7-Logo.png" alt="Logo">
  </a>

  <h3 align="center">My first HPS</h3>

  <p align="center">
    including SoC Embedded Design Suite (EDS) + connecting Linux system + Putty seting
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab7">View Lab7 Demo</a>
  </p>
</p>


<a name="Spec"></a>
<!-- Specification -->
## Specification

* [Objectives](#objectives)
* [Experimental Procedures](#experimental-procedures)
* [License](#license)
* [Let's Get Social](#lets-get-social)
* [Contact](#contact)


<!-- Objectives -->
## Objectives

* Know how to load the program using the ARM processor of the board DE1-SoC. Introducing HPS, the ARM-based hard processor system consisting of processor, peripherals, and memory interfaces with the FPGA fabric using a high-bandwidth interconnect backbone.
* Create the C code file and display "Hello World"


<!-- Experimental Procedures -->
## Experimental Procedures

* Running Linux on the DE1-SoC board
  * Install EDS 13.1 in the same directory of Quartus 13.1
  * Use Win32 Disk Imager to write the Linux BSP image file to micro SD Card
  * Running Linux system by using UART-to-USB
  * Update the driver for connecting the transmission line of UART-to-USB
  * Use Putty for the connection between the PC and DE1-SoC board
  * Set Putty configuration, serial port and speed 115200
  * Observe the state of Linux system at Putty
* My first HPS
  * Build the folder "my_first_hps" in the directory "C:\altera\13.1\embedded\"
  * Build the file "main.c" and the file "Makefile" for link the project
  * Create the environment variable of PC
  * Execute Embedded_Command_Shell.bat in the directory "C:\altera\13.1\embedded\"
  * Type "cd C:/altera/13.1/embedded/my_first_hps" and "make" to generate the file "my_first_hps"
* Compile the file "my_first_hps" using Network without router 
  * Change the network configuration, IP address and sub mask, of PC
  * Type "ifconfig eth0 (IP address) up" at Putty
  * Open CMD of PC to ping (IP address)
  * Type "scp my_first_hps root@(IP address):/home/root" to copy the header file at Embedded_Command_Shell.bat
  * Type "chmod 777 my_first_hps" to change the entitlement of the file at Putty
  * Type "./my_first_hps" to compile the file at Putty, Hello World is on terminal
* Execute the file "my_first_hps" using Network
  * Use an RJ45 cable to connect both PC and DE1-SoC board to ethernet router
  * Type "udhcpc" to query an IP from DHCP server at Putty
  * Open CMD of PC to ping (IP address from DHCP)
  * Type "scp my_first_hps root@(IP address from DHCP):/home/root" to copy the header file at Embedded_Command_Shell.bat
  * Type "chmod 777 my_first_hps" to change the entitlement of the file at Putty
  * Type "./my_first_hps" to executing the file at Putty, Hello World is on terminal
* Execute the file "my_first_hps" using USB
  * Copy the file "my_first_hps" to the USB disk
  * Type "mkdir dir_for_mount" to create a directory for mounting
  * Type "mount -t vfat /dev/sda dir_for_mount" to mount USB
  * Type "./my_first_hps" to executing the file at Putty, Hello World is on terminal
* Execute the file "my_first_hps" using SD card
  * Copy the file "my_first_hps" to SD card
  * Type "mkdir dir_for_mount" to create a directory for mounting
  * Type "mount /dev/mmcblk0p1 dir_for_mount to mount SD card
  * Type "./my_first_hps" to executing the file at Putty, Hello World is on terminal

<p align="right">(<a href="#Spec">back to Specification</a>)</p>


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.


<!-- LET'S GET SOCIAL -->
## Let's Get Social

* [LinkedIn](https://www.linkedin.com/in/%E8%8F%AF%E6%A5%A8-%E5%90%B3-363252241/)
* [Github](https://github.com/trista-csee)


<!-- CONTACT -->
## Contact

吳華楨 Trista Wu - trista.cs11@nycu.edu.tw

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab7](https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab7)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/%E8%8F%AF%E6%A5%A8-%E5%90%B3-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg

