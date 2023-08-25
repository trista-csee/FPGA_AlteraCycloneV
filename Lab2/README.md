<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab2">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab2-Logo.jpg" alt="Logo">
  </a>

  <h3 align="center">Time-of-day clock</h3>

  <p align="center">
    including Electronic clock + BCD counter + 7-segment displays
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab2">View Lab2 Demo</a>
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

Implement a counter to design a real-time clock with reaction-timer.


<!-- Experimental Procedures -->
## Experimental Procedures

* The initial state of the time-of-day clock is 00:00:00
* Switch SW9, SW8 and SW7-0 to set the hour or minute
* When SW9 is 1, SW8 set the hour. When SW9 is 0, SW8 set the minute.
* Set the hour or minute at the positive edge of the signal from SW8
* The time-of-day clock keeps counting while refreshing the hour or minute
* The time-of-day clock returns to the initial state 00:00:00 after counting to 23:59:59
* Pin assignments for DE1-SoC board
* Compile the circuit
* Download the compiled .sof into DE1-SoC board
* Test the circuit by selecting the hour or minute


<!-- Inputs and Outputs -->
## Inputs and Outputs

|Input-1|Input-2|Output-1|Output-2|
|-----------|-------------|------------|------------------------|
|**SW9**|*Select hour or minute*|**HEX5-4**|*Hour (from 0 to 23)*|
|**SW8**|*Set time (positive edge)*|**HEX3-2**|*Minute (from 0 to 59)*|
|**SW7-0**|*Set the value of time*|**HEX1-0**|*Second (from 0 to 59)*|

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

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab1](https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab2)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/%E8%8F%AF%E6%A5%A8-%E5%90%B3-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg

