<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab3">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab3-Logo.jpg" alt="Logo">
  </a>

  <h3 align="center">Multiplexer (8-bit input & 16-bit output)</h3>

  <p align="center">
    including Multiplexer + Multiplier and Adder + 7-segment displays
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab3">View Lab3 Demo</a>
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

Design arithemetic circuits performing the calculation is 8-bit inputs A x B + C x D = 16-bit output S and a carry-out.


<!-- Experimental Procedures -->
## Experimental Procedures

* SW8 select between two sets of inputs A, B or C, D
* SW9 is an active clock edgewrite enable input
* KEY0 is an active-low asynchronnous reset input
* KEY1 is a manual clock input
* KEY2 select the different input in the set
* KEY3 select inputs or sum displayed on HEX3-0
* Pin assignments for DE1-SoC board
* Compile the circuit
* Download the compiled .sof into DE1-SoC board
* Test the circuit by performing some number of multiplications then producing a summation of the results


<!-- Inputs and Outputs -->
## Inputs and Outputs

|Input-1|Input-2|Output-1|Output-2|
|-----------|-------------|------------|------------------------|
|**KEY0**|*Active-low reset*|**LEDR9**|*Carry out*|
|**KEY1**|*Clock*|**HEX3-2**|*A or C*|
|**KEY2**|*Select A or B (C or D)*|**HEX1-0**|*B or D*|
|**KEY3**|*Change display A /B /C /D or S*|**HEX3-0**|*Sum*|
|**SW9**|*Write enable*|||
|**SW8**|*Select A /B or C /D*|||
|**SW7-0**|*The value of input*|||

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

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab3](https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab3)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/hua-chen-wu-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg
