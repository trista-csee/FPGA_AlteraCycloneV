<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab8">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab8-Logo.jpg" alt="Logo">
  </a>

  <h3 align="center">Signal connection in Qsys and compile in Linux</h3>

  <p align="center">
    including Qsys + connecting Linux system + LEDR and 7-segment displays
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab8">View Lab8 Demo</a>
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

* Use Qsys to Control the LEDs and 7-segments of DE1-SoC and connect the ARM core and FPGA core of DE1-SoC board


<!-- Experimental Procedures -->
## Experimental Procedures

* LED control by connecting core of FPGA and ARM
  * Start Qsys to open the Qsys file "soc_system.qsys"
  * Create LED element with PIO (Parallel I/O)
  * Set PIO configuration of LED element in Qsys
  * Generate HDL example and copy ".pio_led_external_connection_export" in Qsys
  * Open "ghrd_top.v", add ".pio_led_external_connection_export" and output parameter is LEDR in Quartus
  * Execute Generation in Qsys
* FPGA compile
  * Open Assignments/Settings, and add "soc_system.qip" from "./quartus labs/Lab8/Altera_TRAN/my_first_hps-fpga_base/soc_system/synthesis/" in Quartus
  * Open Assignments/ Settings, and add "soc_system_timing.sdc" from "./quartus labs/Lab8/Altera_TRAN/my_first_hps-fpga_base/" in Quartus
  * Start Analysis & Synthesis
  * Open Tools/Tcl Scripts and run "hps_sdram_p0_pin_assignments.tcl"
  * Start Compliation
* ARM using Linux system compile
  * Copy the batch file "generate_hps_qsys_header.sh" into the project folder
  * Type "./generate_hps_qsys_header.sh" at Embedded_Command_Shell.bat to produce the header file "hps_0.h" in the directory ".\quartus labs\Lab8\Altera_TRAN\my_first_hps-fpga_base\"
  * Copy the header file "hps_0.h" and create the file "main.c" and "makefile" at the folder ".\quartus labs\Lab8\Altera_TRAN\my_first_hps-fpga_sw\"
  * Compile the header file "hps_0.h" in Putty
* Connecting FPGA and ARM for 7-segment display
  * Start Qsys to open the Qsys file "soc_system.qsys"
  * Create new component defined as 7-segment and name "SEG7_LUT"
  * Add the verilog file "SEG7_LUT.v" in Synthesis Files
  * Set component configuration of 7-segment in Qsys
  * Execute "Analyze Synthsis Files" to check the netlist of 7-segment
* Signal connection in Qsys and compile in Linux
  * Set netlist configuration of 7-segment in Qsys
  * Generate HDL example and copy ".seg7_lut_0_conduit_end_export" in Qsys
  * Open "ghrd_top.v", add ".seg7_lut_0_conduit_end_export" and output parameter is HEX0 in Quartus
  * Execute Generation in Qsys
  * Start Compliation
  * Compile the header file "hps_0.h" in Putty and LED, 7-segment roll 

<p align="right">(<a href="#Spec">back to Specification</a>)</p>


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.


<!-- LET'S GET SOCIAL -->
## Let's Get Social

* [LinkedIn](https://www.linkedin.com/in/hua-chen-wu-363252241/)
* [Github](https://github.com/trista-csee)


<!-- CONTACT -->
## Contact

吳華楨 Trista Wu - trista.cs11@nycu.edu.tw

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab8](https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab8)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/hua-chen-wu-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg

