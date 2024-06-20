<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]]()
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/Lab10/Part3">
    <img src="https://github.com/trista-csee/FPGA_AlteraCycloneV/blob/main/images/Lab10Part3-Logo.jpg" alt="Logo">
  </a>

  <h3 align="center">Adding adjustment on the pixels during the flow of the pixels</h3>

  <p align="center">
    including VGA on DE1-SoC + Connect between the FPGA and VGA + display a frame from .qxp file + count pixels during the iamge flow
    <br />
    <a href="https://github.com/trista-csee/FPGA_AlteraCycloneV/tree/main/LabsDemo/Lab10">View Lab10 Demo</a>
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

* Realize how to access the control signals for videos
* Use .qxp file to output the resolution of the frame 640 * 480 with RGB channels
* Count pixels to add a rectangle during the image flow


<!-- Experimental Procedures -->
## Experimental Procedures

* The VGA protocol mainly consists of 5 input signals: HSYNC Signal, VSYNC Signal, and RGB Signal.
  * HSYNC Signal is the "column synchronization signal"
  * VSYNC Signal is the "row synchronization signal"
  * RGB Signal is the "red, green, blue, color signal"
* VGA scanning a frame of screen is composed of "m row scanning" and "n column filling"
  * A frame of screen display consists of 600 lines scanned from top to bottom and 800 columns filled from left to right.
  * HSYNC Signal is used to control "column filling"
  * VSYNC Signal is used to control "row scan"
  * One row pixel is measured in column pixels: one row pixel = 1056 column pixels
  * One column pixel is measured in time: one column pixel = 25ns, one row pixel = 1056 x 25ns = 2.64us
* Access an encrypted file, .qxp ,which contains a video with I/O to output the resolution of the frame 640 * 480 with RGB channels
  * the video contains only one frame and continuously output the frame
* Use SW0 to choose the original or the adjusted frame for VGA displays
  * the adjusted frame is a rectangle with four corners
  
  

<!-- Inputs and Outputs -->
## Inputs and Outputs

|Input-1|Input-2|Output-1|Output-2|
|-----------|-------------|------------|------------------------|
|**iStart_n**|*Setting to 0 starts to output control the signals and the pixels*|**oData_Enable**|*Setting to 1 displays the frame*|
|**iCLK**|*25.175 MHz Clock*|**oData[23:0]**|*oData[7:0] represents red*|
||||*oData[15:8] represents green*|
||||*oData[23:16] represents blue*|
|**iRST_N**|*Reset signal (Setting to 1 is as ignored signal)*|**HSYNC**|*Column synchronization signal*|
|**SW0**|*Switch the original or the adjusted frame to display*|**VSYNC**|*horizontal synchronization signal*|

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

Project Link: [https://github.com/trista-csee/FPGA_AlteraCycloneV/edit/main/Lab10/Part3](https://github.com/trista-csee/FPGA_AlteraCycloneV/edit/main/Lab10/Part3)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/contributors-1-orange.svg?style=flat-square
[license-shield]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: https://choosealicense.com/licenses/mit
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/hua-chen-wu-363252241/
[product-screenshot]: ./images/projects/portfolio.jpg

