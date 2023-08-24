<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab1">
    <img src="./images/Lab1-Logo.jpg" alt="Logo">
  </a>

  <h3 align="center">Add two 1-digit BCD numbers</h3>

  <p align="center">
    including 7-segment displays + Binary coded decimal + Full adder
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab1">View Lab1 Demo</a>
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

Design combinational circuits performing binary-to-decimal number conversion and binary-coded-decimal (BCD) addition.


<!-- Experimental Procedures -->
## Experimental Procedures

* Use the four-bit adder to produce a four-bit sum and carry-out for A + B
* Conver the result, four-bit sum and carry-out ,into two BCD digits S1S0
* Indicate an error when input A or B is greater than 9
* Pin assignments for DE1-SoC board
* Compile the circuit
* Download the compiled .sof into DE1-SoC board
* Test the circuit by inputing A, B and Carry-in


<!-- Inputs and Outputs -->
## Inputs and Outputs

|Input-1|Input-2|Output-1|Output-2|
|-----------|-------------|------------|------------------------|
|**SW7-4**|*A (binary)*|**HEX5-4**|*Result S1S0 (decimal)*|
|**SW3-0**|*B (binary)*|**HEX3-2**|*A (decimal)*|
|**SW8**|*Carry-in*|**HEX1-0**|*B (decimal)*|
|||**LEDR9**|*Error*|

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

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab1](https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab1)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/%E8%8F%AF%E6%A5%A8-%E5%90%B3-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg
