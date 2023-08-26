<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab4">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab4-Logo.jpg" alt="Logo">
  </a>

  <h3 align="center">Counter-like circuit (10-module)</h3>

  <p align="center">
    including Counter + 7-segment displays
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab4">View Lab4 Demo</a>
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

Design a 10-module counter-like circuit.


<!-- Experimental Procedures -->
## Experimental Procedures

* Two inputs w1w0 = 00, the count remains the same
* Two inputs w1w0 = 01, the count is incremented by 1
* Two inputs w1w0 = 10, the count is incremented by 2
* Two inputs w1w0 = 11, the count is decremented by 1
* All changes take place on the negative edge trigger
* SW2-1 select input w1 and w0
* SW0 is an active-low synchronous reset
* KEY0 is a manual clock
* Pin assignments for DE1-SoC board
* Compile the circuit
* Download the compiled .sof into DE1-SoC board
* Test the circuit by applying some inputs and observing the output display


<!-- Inputs and Outputs -->
## Inputs and Outputs

|Input-1|Input-2|Output-1|Output-2|
|-----------|-------------|------------|------------------------|
|**SW2**|*Input (w1)*|**HEX0**|*Count (0-9 in cycle)*|
|**SW1**|*Input (w0)|||
|**SW0**|*Active-low reset*|||
|**KEY0**|*Clock (negative edge)*|||

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

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab4](https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab4)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/%E8%8F%AF%E6%A5%A8-%E5%90%B3-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg

