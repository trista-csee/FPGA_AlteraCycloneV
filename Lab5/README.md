<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab5">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab5-Logo.png" alt="Logo">
  </a>

  <h3 align="center">Substitute dual-port memory by single-port memory</h3>

  <p align="center">
    including Single-port RAM + Read and Write RAM + 7-segment displays
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab5">View Lab5 Demo</a>
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

Design circuits using only one address port RAM to select either a read or write address.


<!-- Experimental Procedures -->
## Experimental Procedures

* Use the MegaWizard Plug-in Manager to create a 1-port RAM
* Specify a memory initialization file (MIF)
* Allow In-System Memory Content Editor to capture and update content independly of the system clock 
* The operation result is examined by the In-System Memory Content Editor
* The initial values of RAM is 0
* Pin assignments for DE1-SoC board
* Compile the circuit
* Download the compiled .sof into DE1-SoC board
* Test the circuit by changing some memory values and observing the data properly displayed both on the 7-segment displays on the board and in the In-System Memory Content Editor


<!-- Inputs and Outputs -->
## Inputs and Outputs

|Input-1|Input-2|Output-1|Output-2|
|-----------|-------------|------------|------------------------|
|**CLOCK_50**|*Clock*|**LEDR0**|*Write signal*|
|**SW4-0**|*5 bit write address*|**HEX3-2**|*5 bit address display (in hexadecimal format)*|
|**SW7-0**|*8 bit write data*|**HEX1-0**|*8 bit read out data (in hexadecimal format)*|
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

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab5](https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab5)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/%E8%8F%AF%E6%A5%A8-%E5%90%B3-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg

