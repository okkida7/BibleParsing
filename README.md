<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

<!-- PROJECT LOGO -->

<h3 align="center">Bible Parsing</h3>

  <p align="center">
    <br />
    <a href="https://github.com/okkida7/BibleParsing"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/okkida7/BibleParsing">View Demo</a>
    ·
    <a href="https://github.com/okkida7/BibleParsing/issues">Report Bug</a>
    ·
    <a href="https://github.com/okkida7/BibleParsing/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The goal of this project is to identify Greek grammar in each verse of the Bible and parse semantically equivalent sentences from different languages into their corresponding grammar. Specifically we will first compare books in [morphological Greek New Testament(mGNT)](https://www.biblegateway.com/versions/SBL-Greek-New-Testament-SBLGNT/) and [New American Standard Bible 1995(NASB1995)](https://www.biblegateway.com/versions/New-American-Standard-Bible-NASB1995/). Same method can be applied to other languages.
 <br />
The text resources come from [blueletterbible.org](blueletterbible.org) and [biblegateway.com](blueletterbible.org)
<br /> 
For detailed information about Greek grammar, refer to [Greek Grammar](https://www.blueletterbible.org/assets/pdf/grammars/Simplified_Greek_Grammar_v5.pdf). 

<!--  Here's a blank template to get started: To avoid retyping too much info. Do a search and replace with your text editor for the following: `github_username`, `repo_name`, `twitter_handle`, `linkedin_username`, `email`, `email_client`, `project_title`, `project_description` -->

<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

[Jupyter Notebook](https://jupyter.org/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

As well as Python 3, you will need to install [beautifulsoup4 4.10.0](https://pypi.org/project/beautifulsoup4/#files):
* pip
  ```sh
  pip install beautifulsoup4
  ```
JupyterLab is recommended. To install, see [Installation of the Jupyter Software](https://jupyter.org/install).

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage
If you want to see the English text in forward line(original word order), use [BibleParsing_English.ipynb](https://github.com/okkida7/BibleParsing/blob/screenshots/BibleParsing_English.ipynb).
<br />
If you want to see the Greek text in forward line, use [BibleParsing_Greek.ipynb](https://github.com/okkida7/BibleParsing/blob/screenshots/BibleParsing_Greek.ipynb).
<br />
Go to [BiblrGateway](https://www.biblegateway.com/) and enter the <book/passage/verse> and the version name.
<br />
For English version, here is an example:
1. ![BibleGateway url](/../<screenshots>/path/to/biblegateway_e.png?raw=true "BibleGateway url")
2. Open BibleParsing_English.ipynb. Copy and paste the url to the first user input in the ipynb file. <br />![user_input1](/../<screenshots>/path/to/userinput1.png?raw=true "user_input1")
3. Go to [BlueLetterBible](https://www.blueletterbible.org/) and enter the corresponding <book/passage/verse> and select language mGNT. <br /> ![blb1](/../<screenshots>/path/to/blb1.png?raw=true "blb1")
4. Right click 'TOOLS'. <br /> ![blb2](/../<screenshots>/path/to/blb2.png?raw=true "blb2")
5. Under 'INTERLINEAR', right click 'Rev Inline'. This step will convert the text to Greek-reverse and English-forward order. ![blb3](/../<screenshots>/path/to/blb3.png?raw=true "blb3")
6. Right click 'View Options', make corresponding changes as shown in the screenshot. <br />![blb4](/../<screenshots>/path/to/blb4.png?raw=true "blb4")
7. Right click the arrow next to 'Rev Inline'. If you want to see the whole chapter, right click 'Full Chapter'. Copy every word from left to right and top to bottom and paste to a text file. IMPORTANT: make sure to include every word including empty space, exclude any other irrelevant texts. Else the program will not run properly.<br />![blb5](/../<screenshots>/path/to/blb5.png?raw=true "blb5")
8. Your text file should look like this: <br />![txt1](/../<screenshots>/path/to/txt1.png?raw=true "txt1")<br />Make sure the word type is always English-Greek-ParsingCode from top to bottom and this pattern is repeated until the end.
9. If you have cloned the repository, upload the text file to your branch. If you have downloaded the code to your desktop, make sure your text file and ipynb file are in the same directory.
10. Enter txt file name in BibleParsing_English.ipynb. Include '.txt'. Then enter the starting verse number and the ending verse number. Here is an example: <br />![userinput2](/../<screenshots>/path/to/userinput2.png?raw=true "userinput2")
11. The output should be color-coded, line by line with verse number and punctuations. <br />![output1](/../<screenshots>/path/to/output1.png?raw=true "output1")
<br />
For Greek version, go to BibleGateway and change the version to 'SBL GREEK NEW TESTAMENT(SBLGNT)'. go to BlueLetterBible and this time right click 'Forward Inline'. Repeat the same every other step for BibleParsing_Greek.ipynb.
<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

BibleParsing_English
- Load English bible book from biblegateway.com
- Initial clean (includes removing footnotes such as "(A)","[a]", unwanted annotations)
- Get index from texts in order to form separate sentences
- Load bible book from blueletterbible.org and arrange text into group of 3: (English, Greek, Parsing Code)
- Apply color
    - Use dictionary to assign words with colors<br />![parsecode](/../<screenshots>/path/to/parsecode.png?raw=true "parsecode")
    - Define function to convert parsing code to color code
- Complete token for each verse in the paragraph
    - Get user's paragraph according to starting verse number and ending verse number
    - Get token from txt file
    - Get list of verses with correct tokens that match the mapping text file
    - Define token(string,item) 
          - string: the original sentence
          - item: the token we want to apply to each word in sentence
- Get number's index for user's paragraph
- Print complete color-coded user paragraph with verse number, punctuation, and line break

BibleParsing_Greek
- Similar step
- More handling on texts because the encoding is different for the same word in blueletterbible.org and biblegateway


See the [open issues](https://github.com/okkida7/BibleParsing/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Alexis Jin - xj606@stern.nyu.edu

Project Link: [https://github.com/okkida7/BibleParsing](https://github.com/okkida7/BibleParsing)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* Justin Alfred has made the following Hebrew and Greek Grammars available to Blue Letter Bible.[Greek Grammar](https://www.blueletterbible.org/assets/pdf/grammars/Simplified_Greek_Grammar_v5.pdf). 

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/okkida7/BibleParsing.svg?style=for-the-badge
[contributors-url]: https://github.com/okkida7/BibleParsing/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/okkida7/BibleParsing.svg?style=for-the-badge
[forks-url]: https://github.com/okkida7/BibleParsing/network/members
[stars-shield]: https://img.shields.io/github/stars/okkida7/BibleParsing.svg?style=for-the-badge
[stars-url]: https://github.com/okkida7/BibleParsing/stargazers
[issues-shield]: https://img.shields.io/github/issues/okkida7/BibleParsing.svg?style=for-the-badge
[issues-url]: https://github.com/okkida7/BibleParsing/issues
[license-shield]: https://img.shields.io/github/license/okkida7/BibleParsing.svg?style=for-the-badge
[license-url]: https://github.com/okkida7/BibleParsing/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/alexisjin0219
[product-screenshot]: images/screenshot.png
