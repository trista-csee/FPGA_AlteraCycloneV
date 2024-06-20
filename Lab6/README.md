<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab6">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab6-Logo.jpg" alt="Logo">
  </a>

  <h3 align="center">Four instructions (mv /mvi /add /sub) processor including memory</h3>

  <p align="center">
    including Two clock + Single-port ROM + Read ROM and Write Registerfile  + 7-segment displays
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab6">View Lab6 Demo</a>
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

Design the processor with four instructions (mv /mvi /add /sub).


<!-- Experimental Procedures -->
## Experimental Procedures

* Use the counter to read the contents of successive addresses in the memory
* The contents read from the memory are provided to the processor as a stream of instructions
* Use two separate clock signal, PClock and MClock, for the processor and the memory
* Read properly out of ROM and executed by the processor
* Pin assignments for DE1-SoC board
* Compile the circuit
* Download the compiled .sof into DE1-SoC board
* Test the circuit by using the specified MIF file with processor instructions


<!-- Inputs and Outputs -->
## Inputs and Outputs

|Input-1|Input-2|Output-1|Output-2|
|-----------|-------------|------------|------------------------|
|**KEY0**|*Resetn*|**LEDR7-0**|*processor bus wires*|
|**KEY1**|*MClock*|**HEX5-4**|*DIN*|
|**KEY2**|*PClock*|**HEX3-2**|*value of R0*|
|||**HEX1-0**|*value of R1*|

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

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab6](https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab6)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/hua-chen-wu-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg
