l13-hw06
* Status: Final
* CodePen: <https://codepen.io/chindraba-ga/pen/>
* Live page: <https://fewd.chindraba.work/lessons/l13-hw06/index.html>

Contents
================================================================================

* Description
* Copyright and License
  * The MIT License

Description
================================================================================

Lesson 13: Assignment: CitiPix

Our goal is to create a background switching search form. Your input field will
take values from the form and match them in JS. When there is a match, the
background image should change.

The starter code is:

- HTML

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="utf-8">
        <meta name="description" content="Citipix example">
        <meta name="keywords" content="one, two, three">
        <title>City Background</title>
    </head>
    <body>
        <header class="citipix-container">
        <h1 class="citipix-title">CitiPix</h1>
        <p class="citipix-description">Find your city to change the background...</p>
        </header>
    <form id="citipix-form"> 
        <input type="text" id="city-type" placeholder="Enter a city name...">
        <input type="submit" value="Update" id="submit-btn">
    </form>
    <script src="js/index.js" type="text/javascript"></script>
    </body>
    </html>

- CSS

    /******************************************
    /* BASE STYLES
    /*******************************************/

    body {
      color: #000;
      font-size: 12px;
      line-height: 1.4;
      font-family: Helvetica, Arial, sans-serif;
      background: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/citipix_skyline.jpg) no-repeat center center fixed;
      background-size: cover;
    }


    /******************************************
    /* LAYOUT
    /*******************************************/

    /* Center the container */
    .container {
        width: 960px;
        margin: auto;
      padding-top: 5em;
    }

    header {
      background-image: linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.7));
      padding: 15px 0;
    }

    .citipix-container {
      text-align: center;
      color: #fff;
      font-family: helvetica, arial, sans-serif;
    }

    .citipix-title {
      font-size: 32px;
    }

    .citipix-description {
      font-size: 22px;
    }

    #citipix-form {
      align-items: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
      height: 350px;
    }

    @media (min-width: 1100px) {
      #citipix-form {
        flex-direction: row;
      }
    }

    #city-type {
      border: 1px solid #111;
      color: #6b6b6c;
      font-size: 24px;
      height: 72px;
      margin: 0 0 25px 0;
      padding: 0px 30px;
      width: calc(100% - 120px);
    }

    @media (min-width: 800px) {
      #city-type {
        font-size: 38px;
        width: 680px;
      }
    }

    @media (min-width: 1100px) {
      #city-type {
        margin: 0 25px 0 0;
      }
    }

    #submit-btn {
      background: #ffe500;
      color: #000;
      cursor: pointer;
      font-size: 24px;
      font-weight: bold;
      text-transform: uppercase;
      text-align: center;
      transition: 0.4s ease-in-out;
      width: 250px;
      height: 72px;
    }

    @media (min-width: 1100px) {
      #submit-btn {
        font-size: 32px;
      }
    }

    #submit-btn:hover {
      background: #fff600;
    }



    /* Styles you can add into the document dynamically with JS - hint, hint ;) */
    .nyc {
      background-image: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/nyc.jpg)
    }
    .sf {
      background-image: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/sf.jpg)
    }
    .la {
      background-image: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/la.jpg)
    }
    .austin {
      background-image: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/austin.jpg)
    }
    .sydney {
      background-image: url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/sydney.jpg)
    }


Copyright and License
================================================================================

The MIT license applies to all the code within this repository.

Copyright © 2020  Chindraba (Ronald Lamoreaux)
            <upskill@chindraba.work>
- All Rights Reserved

The MIT License

Permission is hereby granted, free of charge, to any person obtaining a
copy of this software and associated documentation files (the "Software"),
to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGE MENT. IN NO EVENT SHALL
THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
DEALINGS IN THE SOFTWARE.
