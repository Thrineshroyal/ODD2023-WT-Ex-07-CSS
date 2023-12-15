# AIM :
## To interpret the functionalities of media queries in html and css.
## Developed By : T.Thrinesh Royal
## Register Number : 212223230226
# Objective 1 :
### Using CSS media queries to modify the webpage's color scheme.
## Step 1 :
Define Default Color Scheme:

Set the default background color, text color, and link color for the entire webpage.
## Step 2 :
Media Query for Small Screens:

Use a media query (@media (max-width: 600px)) to target screens with a maximum width of 600 pixels.
Change the background color, text color, and link color to create a different color scheme suitable for smaller screens.
## Step 3 :
Media Query for Dark Mode Preference:

Use a media query (@media (prefers-color-scheme: dark)) to target devices with a dark mode preference.
Adjust the background color, text color, and link color to create a dark mode color scheme.
## Step 4 :
Apply Styles:

Apply the defined color schemes to the respective elements using CSS.
## Code :
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Color Scheme</title>

  <style>
/* Default Color Scheme */
body {
  background-color: #f4f4f4;
  color: #333;
}

a {
  color: #007bff;
}

/* Small Screen Adaptation */
@media (max-width: 600px) {
  body {
    background-color: #333;
    color: #f4f4f4;
  }

  a {
    color: #28a745;
  }
}

/* Dark Mode Preference */
@media (prefers-color-scheme: dark) {
  body {
    background-color: #000;
    color: #fff;
  }

  a {
    color: #17a2b8;
  }
}
  </style>
</head>

<body>
  <h1>Webpage created using CSS MEDIA QUERIES to modify the webpage's color scheme.</h1>
 

  <!-- Link to demonstrate blue color -->
  <a href="www.saveetha.ac.in">SAVEETHA.COM</a>
</body>

</html>

```
# Output :
### Webpage's color scheme when it is on larger devices like pcs and desktops.


![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/bba29784-6dd6-4137-b0e7-8014847e7ade)


### Webpage's color scheme when it is on smaller devices like smart phones.


![WhatsApp Image 2023-12-12 at 18 48 48_01b69980](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/0a0ebfba-7b43-46e3-927f-3dfd3264c87b)

# Objective 2 :
### Using CSS media queries to modify mobile and desktop styles.
## Step 1 :
Define Desktop Styles:

Set default styles for desktop devices, including font size, background color, and container styles.
## Step 2 :
Media Query for Mobile Devices:

Use a media query (@media screen and (max-width: 599px)) to target screens with a maximum width of 599 pixels.
Adjust font size, background color, and container styles for a mobile-friendly layout.
## Step 3 :
Apply Styles:

Apply the defined styles to the corresponding HTML elements using CSS.
## Step 4 :
Test Responsiveness:

Test the webpage on both desktop and mobile devices to ensure the styles adapt based on the screen width.
## Step 5 :
Refine Styles as Needed:

Refine styles based on testing feedback, making adjustments for better responsiveness and aesthetics.
## Code :
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style type="text/css">
    /* Styles for desktop devices */
    body {
      font-size: 16px;
      background-color: #f2f2f2;
      color: #333;
    }

    .container {
      max-width: 960px;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      border: 1px solid #ddd;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    /* Media query for mobile devices with width less than 600px */
    @media screen and (max-width: 599px) {
      body {
        font-size: 14px;
        background-color: #e6e6e6;
        color: #555;
      }

      .container {
        padding: 10px;
        background-color: #f9f9f9;
        border: 1px solid #ccc;
        box-shadow: none;
      }

      .device-specific {
        font-weight: bold;
        color: #ff5733;
      }
    }
  </style>
  <title>Responsive Design Example</title>
</head>
<body>
  <div class="container">
    <h1>Responsive Design Example</h1>
    <p>This is some text that will be visible on all devices. The background color and font size will change based on the screen width.</p>
    <p class="device-specific">This text will have different styles on different devices. It's now bold and has a different color on mobile devices.</p>
  </div>
</body>
</html>


```
# Output :
## Webpage Design when opened on large width devices like pc
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/0367377e-ffd9-427e-967e-db676a668d55)

## Webpage Design when opened on small width devices like mobile phones
![WhatsApp Image 2023-12-12 at 20 25 10_216807ea](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/111ed8a6-5c68-47fa-9170-367e1fab62a6)

# Objective 3 :
### Using CSS media queries to represent orientation scheme.
## Step 1 :
Define Styles for Portrait and Landscape:

Set default styles for both portrait and landscape orientations.
## Step 2 :
Media Query for Portrait Orientation:

Use a media query (@media (orientation: portrait)) to target devices in portrait orientation.
Adjust background color or other styles to differentiate the presentation.
## Step 3 :
Media Query for Landscape Orientation:

Use a media query (@media (orientation: landscape)) to target devices in landscape orientation.
Adjust background color or other styles to differentiate the presentation.
## Step 4 :
Apply Styles:

Apply the defined styles to the corresponding HTML elements using CSS.
## Step 5 :
Test on Different Devices:

Test the webpage on devices with varying orientations to ensure the styles adapt correctly.
## Code :
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Orientation Scheme</title>

  <style>
/* Styles for portrait orientation */
@media (orientation: portrait) {
  body {
    background-color: #e6f7ff; /* Light blue background for portrait orientation */
  }

}

/* Styles for landscape orientation */
@media (orientation: landscape) {
  body {
    background-color: rebeccapurple; /* Light red background for landscape orientation */
  }

}

  </style>
</head>

<body>
  <h1>Webpage that demonstrates the orientation scheme on devices</h1>


</body>

</html>

```
# Output :
## Webpage's background colour is purple when opened on landscape orientation (pc)
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/da57afc4-46ed-4d79-a3d7-a9aa59b38ef6)

## Webpage's background colour changes to light green when opened on portriat orientation (mobile phone)
![WhatsApp Image 2023-12-12 at 19 46 40_2ea08ce5](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/a05d674c-eb3a-47d5-a65b-1c9a67bb1acf)

# Objective 4 :
## Responsive Typography using CSS Media queries
## Step 1 :
Define Default Typography:

Set default font size and line height for all devices.
## Step 2 :
Media Query for Medium Devices:

Use a media query (@media screen and (min-width: 600px) and (max-width: 899px)) to target screens with widths between 600px and 899px.
Adjust font size and line height for a medium-sized screen.
## Step 3 :
Media Query for Large Devices:

Use a media query (@media screen and (min-width: 900px)) to target screens with widths of 900px and above.
Adjust font size and line height for larger screens.
## Step 4 :
Apply Styles:

Apply the defined font size and line height to the HTML elements using CSS.
## Step 5 :
Test Responsiveness:

Test the typography on different devices to ensure readability and aesthetics.
# Code :
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style type="text/css">
    /* Default styles for all devices */
    body {
      font-size: 16px;
      line-height: 1.6;
      margin: 20px;
    }

    /* Media query for devices with width between 600px and 899px */
    @media screen and (min-width: 600px) and (max-width: 899px) {
      body {
        font-size: 18px;
        line-height: 1.5;
      }
    }

    /* Media query for devices with width 900px and above */
    @media screen and (min-width: 900px) {
      body {
        font-size: 20px;
        line-height: 1.4;
      }
    }
  </style>
  <title>Responsive Typography Example</title>
</head>
<body>
  <h1>Responsive Typography Example</h1>
  <p>
    This is some text on the webpage. The font size and line spacing will adjust based on the screen width.
  </p>
  <p>
    This example webpage design is adjusted automatically based on the device type and maximum width
  </p>
</body>
</html>

```

# Output :

## Font size is 18px and line height is 1.6 when opened on larger devices like pc

![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/25678537-6698-466b-b939-78d1f5add950)

## Font size is reduced to 14px on devices with a maximum width of 600px like mobile phones 

![WhatsApp Image 2023-12-12 at 20 35 11_d59cfb3f](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/c4f2cbe6-57ec-4af8-a13c-d8d4d9f56287)

# Objective 5 :
## Print-friendly styles for web pages using CSS media quries
## Step 1 :
Define Default Styles:

Set default background color, text color, and link color for the webpage.
## Step 2 :
Media Query for Print Styles:

Use a media query (@media print) to target styles specifically for printing.
Adjust background color, text color, and link color for a print-friendly presentation.
## Step 3 :
Hide Non-Essential Elements:

Use CSS to hide non-essential elements that are not necessary for printing, using display: none.
## Step 4 :
Apply Print Styles:

Apply the defined print styles to the HTML elements using CSS.
## Step 5 :
Print Testing:

Print the webpage or use browser print preview to check how the styles appear on a printed page.
## Code :
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Print-friendly Styles</title>

  <style>
    /* Default styles for the webpage */
    body {
      background-color: #f4f4f4; /* Light gray background */
      color: #333; /* Dark gray text color */
    }

    a {
      color: #007bff; /* Blue link color */
    }

    .non-essential {
      display: block; /* Visible by default */
    }

    /* Media query for print styles */
    @media print {
      body {
        background-color: #fff; /* White background for printing */
        color: #000; /* Black text color for printing */
      }

      a {
        color: #17a2b8; /* Cyan link color for printing */
      }

      .non-essential {
        display: none; /* Hide non-essential elements for printing */
      }

    }
  </style>
</head>

<body>
  <h1>Print-friendly Styles Example</h1>
  <p>This is the content of your webpage.</p>
  <p class="non-essential">This is a non-essential element.</p>
  <p>More content...</p>
</body>

</html>

```
# Output :
## Webpage Design when opened in view-mode
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/ba01736d-6297-4baf-99fa-fd57a5ecf6d1)

## Webpage Design changes when opened in print-mode
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/57b44ce1-0db6-4fb0-9ec2-735ef9750572)

## Non-essential elements are not displayed in print-mode

# Objective 6 :
## Dark mode Implementation using CSS media queries
## Step 1 :
Define Default Color Scheme for Light Mode:

Set the default background color and text color for the entire webpage.
## Step 2 :
Media Query for Dark Mode Preference:

Use a media query (@media (prefers-color-scheme: dark)) to target devices with a dark mode preference.
Adjust the background color and text color to create a dark mode color scheme.
## Step 3 :
Apply Styles:

Apply the defined color schemes to the corresponding HTML elements using CSS.
## Step 4 :
Test on Devices with Dark Mode Preference:

Test the webpage on devices with dark mode preferences to ensure the dark mode styles are applied.
## Step 5 :
Toggle Dark Mode Setting:

If applicable, toggle the system's dark mode setting and observe the webpage adapting to the change.
# Code :
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dark Mode Example</title>

  <style>
    /* Default color scheme for light mode */
    body {
      background-color: #f4f4f4; /* Light gray background */
      color: #333; /* Dark gray text color */
    }

    /* Additional styles for light mode as needed */

    /* Dark mode preference */
    @media (prefers-color-scheme: dark) {
      body {
        background-color: #000; /* Dark background for dark mode */
        color: #fff; /* Light text color for dark mode */
      }

    }
  </style>
</head>

<body>
  <h1>Dark Mode Example</h1>
  <p>This webpage dynamically adapts to the user's system preference for dark mode.</p>
  <p>Toggle your system's dark mode setting to see the changes!</p>
</body>

</html>

```

## Webpage is Displayed in light mode when device is running on light theme
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/e04ca496-1b5d-4c0c-a81c-7f6e7aa4ea58)

## Webpage is Displayed in dark mode when deivce is running on dark mode
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-07-CSS/assets/80164014/6af765c7-db2b-41d8-91b6-876ba5585b2b)

# Result :
## Therefore, functionalities of CSS media queries are clearly demonstrated using examples for each type.
