<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab9">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab9-Logo.jpg" alt="Logo">
  </a>
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab9">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab9-Logo2.jpg" alt="Logo2">
  </a>

  <h3 align="center">Reading and Writing control of ARM DDR3</h3>

  <p align="center">
    including FPGA configuration mode switch + Read and Write ARM DDR3 + 7-segment displays
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab9">View Lab9 Demo</a>
  </p>
</p>


<a name="Spec"></a>
<!-- Specification -->
## Specification

* [Objectives](#objectives)
* [Experimental Procedures](#experimental-procedures)
* [Inputs and Outputs](#inputs-and-outputs)
* [License](#license)
* [Let's Get Social](#lets-get-social)
* [Contact](#contact)


<!-- Objectives -->
## Objectives

* Change the FPGA configuration scheme to FPPx32 and use SD card to load the FPGA configuration file into memory
* Use Qsys to generate ARM DDR3 memory module and execute read and write control of ARM DDR3


<!-- Experimental Procedures -->
## Experimental Procedures

* FPGA board physical configuration
  * Toggle the MSEL switch to MSEL[4:0] = 01010 to change the FPGA configuration scheme so that the FPGA access DDR3 through the FPGA Bridge  
* Generate a DDR3 module in Qsys
  * Execute "DE1SoC_SystemBuilder.exe", generate a new project with HPS inputs and outputs
  * Add the hard processor system IP and set the HPS configuration in Qsys
  * Add the clock bridge IP and set the clock bridge configuration in Qsys
  * Add the address span extender IP and set the address span extender configuration in Qsys
  * Remove clk_0 and connect the HPS, clock bridge and address span extender in Qsys
  * Save all configuration as "soc_system.qsys" and generate HDL design file
  * Generate HDL example and copy the instantiation template in Qsys
  * Open "DE1_SOC.v", add the instantiation templat and correct the output parameter in Quartus
  * Open Assignments/Settings, and add "soc_system.qip" from "./quartus labs/LAB9/DE1SoC_SystemBuilder/CodeGenerated/DE1_SOC/DE1_SOC/soc_system/synthesis/" in Quartus
  * Open Assignments/Settings, and add "DE1_SOC.SDC" from "./quartus labs/LAB9/DE1SoC_SystemBuilder/CodeGenerated/DE1_SOC/DE1_SOC/" in Quartus
* Read and Write control of ARM DDR3
  * Call the DDR3 memory module produced in Qsys
  * Read and write DDR3 content to display on the 7-segment displays
  * Start Analysis & Synthesis
  * Open Tools/Tcl Scripts and run "hps_sdram_p0_parameters.tcl" and "hps_sdram_p0_pin_assignments.tcl"
  * Start Compliation to produce the sof file
  * Run "sof_to_rbf.bat" to convert the sof file to "soc_system.rbf"
  * Copy the file "soc_system.rbf" into SD card and insert SD card into the DE1-SoC board


<!-- Inputs and Outputs -->
## Inputs and Outputs

|Input-1|Input-2|Output-1|Output-2|
|-----------|-------------|------------|------------------------|
|**CLOCK_50**|*Clock*|**HEX3-2**|*8 bit write in data (in hexadecimal format)*|
|**SW7-0**|*8 bit data in*|**HEX1-0**|*8 bit read out data (in hexadecimal format)*|
|**SW9**|*Write enable*|||

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

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab9](https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab9)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/%E8%8F%AF%E6%A5%A8-%E5%90%B3-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg
