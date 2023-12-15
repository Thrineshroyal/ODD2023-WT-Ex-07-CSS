# Ex-07-CSS
# Name: T.Thrinesh Royal
# Ref.no:212223230226
# Aim:
# Ex-7(i):

Using CSS media queries, modify the webpage's color scheme with the following requirements:

Default Color Scheme: Background color: Light gray (#f4f4f4) Text color: Dark gray (#333) Link color: Blue (#007bff) Small Screen Adaptation (Max-width: 600px):

Change the background color to dark gray (#333) Change the text color to light gray (#f4f4f4) Change the link color to light green (#28a745)

Dark Mode Preference:

If the user has set their device to dark mode, override the above styles with the following: Background color: Black (#000) Text color: White (#fff) Link color: Cyan (#17a2b8)
# Steps:

## Step1:
Meet the requirements for the default mode or light mode
## Step2:
Choose a device which is smaller in size of mobilephone of 600px and meet the prefered requirements
## Step3:
Meet the requirements for the prefered darker mode

# Code:
media.html:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="pj.css">
   
</head>
<body>
    <fieldset>
      <p align="center">
        <legend align="center"><b>This is My Web Page</b></legend>
        
        <p align="center">Hi, This is Jeshwanth Kumar from the dept of Aiml</p>
      </p>
    </fieldset>

    <hr>
    <a href="https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS.git">https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS.git</a>
<br>
    <footer>~Created By @P.Jeshwanth Kumar</footer>
</body>
</html>

```
pj.css:
```
html {
    font-size: 50px;
    color: #333;
    background-color: #f4f4f4;
}

a {
    color: #007bff;
}
@media (max-width: 600px) {
            html {
                background-color: #333;
                color: #f4f4f4;
                a {
                    color: #28a745;
            }
            }
        
        }

@media (prefers-color-scheme: dark) {
    html {
        font-size: 50px;
        background: #333;
        color: white;
    }
 a {
        color: #17a2b8; 
 }
}

footer {
    font-size: x-large;
}

```




# Output(i):
light mode:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/7a5c656b-a99f-4bb2-8f24-e81046187426)






Dark mode:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/7e5224fd-e635-4d56-b294-79784873f8b5)



Smaller screen:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/865355b6-7705-4792-9dc4-8be4f681c8c7)
# Ex-7(ii):
## Aim: To use a media query in CSS to apply different styles to a webpage for mobile devices (with widths less than 600px) and desktop devices (with widths greater than or equal to 600px) by providing an example CSS snippet to demonstrate your answer.
## Step 1:
Start a html project
## Step 2:
Create a css file in the same folder in which html file is created
## Step 3:
inside html code give href link of the css code
## Step 4:
meet the requirements given in the question
## Step 5:
run the program with prefered screen width
# Program:
```
2.css
html {
    font-size: 50px;
    color: #333;
    background-color: orange;
}

a {
    color: #007bff;
}
@media (max-width: 600px) {
            html {
                background-color: pink;
                color: #f4f4f4;
                a {
                    color: #28a745;
            }
            }
        
        }
```
# Output(ii):
default:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/848a0735-f2fd-4a91-acd2-20a1b4db98ea)
max screen width of 600px:
![Screenshot 2023-12-12 222159](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/686695d4-66b0-4d15-aeb4-7b42a66ed45d)

# Ex-7(iii):
## Aim:Explain how you can use CSS media queries to apply different styles based on the orientation (landscape or portrait) of the device. Provide a CSS example where you change the background color of the body based on the orientation.

## Step1:
start a html project
## Step 2:
create a css file in the same folder in which file is created,give the href link in the html code
## Step3:
Define a CSS media query for each orientation. The syntax for a media query is @media (orientation: value), where value can be either portrait or landscape.
## Step 4:
You can change background color of it
## Step4:
Run the html program
# Program
```

3.css
@media (orientation: potrait) {
            html {
                background-color: white;
                color: black;
                a {
                    color: purple;
            }
            }
        
        }
        @media (orientation: landscape) {
            html {
                background-color: yellow;
                color: black;
                a {
                    color: #28a745;
            }
            }
        
        }      
```
# Output:
landscape:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/0738cfdf-faca-45d8-9889-19c3741ab666)
potrait:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/8ec31405-bb54-43a8-a259-09295a7afced)
## Ex-7(iv):
## Aim:To describe how you would use media queries to adjust typography (like font size and line spacing) on a website to improve readability across different device sizes, from mobile phones to large desktop monitors. Include a CSS code snippet in your explanation.
## Step1:
start a html project
## Step 2:
create a css file in the same folder in which file is created,give the href link in html code
## Step 3:
give different font sizes for different screen sizes accordingly
## Step4:
adjusting different colors for different screen width
# Step5:
Run the html program
# Program:
```
4.css
html {
    font-size: 20px;
    color: yellow;
    background-color: purple;
}

a {
    color: yellow;
}

@media (min-width: 600px) {
            html {
                font-size: 50px;
                background-color: pink;
                color: #f4f4f4;
                a {
                    color: #28a745;
                    
                        
            }
            }
           
        
        }
@media (min-width: 800px) {
            html {
                font-size: 80px;
                background-color: red;
                color: #f4f4f4;
                a {
                    color: #28a745;
                    
                        
            }
            }
           
        
        }
```
# Output(iv):
min-width=800px:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/4911c611-af9d-44cf-bc8a-f0f0044a1b10)


max-width=600px:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/fc641ee0-1a81-4488-b021-fdacf044fefe)




default:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/8e3a7325-4729-454f-92d8-caf9dcea0e40)

# Ex-7(v):
# Aim:Media queries can be used to provide print-friendly styles for web pages. How would you use a media query to change the styling of a webpage when it is printed, such as changing the background to white and hiding non-essential elements Provide a CSS example.
## Step1:
start a html project
## Step 2:
create a css file in the same folder in which file is created,give href link in html program
## Step3:
after creating a css file give Inside each media query block, adjust the styles for the identified elements. You can change the background to white and hide non-essential elements.
## Step4:
test the html file
## Step5:
run the html program
# Program:
```
5.css
html {
    font-size: 50px;
    color: #333;
    background-color: #f4f4f4;
}

a {
    color: #007bff;
}
@media print {
            html {
                font-size: 20px;
                background-color: #333;
                color: #f4f4f4;
                a {
                    color: #28a745;
                    .non-essential {
                        display: none;
                    }
            }
            }
        
        }
```
# Output(v):
default:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/12522601-a6fd-45eb-9ca0-d9c59ea131be)
non essential:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/bbd9cfe7-7a2f-4efb-925f-48cb0ec564a4)
# Ex-7(vi):
# Aim:With the increasing popularity of dark mode in user interfaces, explain how you would use a media query to detect if the user has set their system to prefer a dark color scheme. Provide an example of how you would change the background and text colors of a website based on this preference.
## Step1:
start a html project
## Step 2:
create a css file in the same folder in which file is created,give href link in html program
## Step 3:
using media queries set the preference to dark mode and night mode
## Step 4:
change the background color and font color to different
## Step 5:
run the html program
# Program:
```
6.css
html {
    font-size: 50px;
    color: #333;
    background-color: #f4f4f4;
}

a {
    color: #007bff;
}


@media (prefers-color-scheme: dark) {
    html {
        font-size: 50px;
        background: #333;
        color: white;
    }
 a {
        color: #17a2b8; 
 }
}

```
# Output(vi):
lightmode:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/a6920150-8575-4ae9-8081-e91fd222ddb4)


darkmode:
![image](https://github.com/Jeshwanthkumarpayyavula/ODD2023-WT-Ex-07-CSS/assets/145742402/7bc7a6f6-526a-4f2b-bbda-71b3f892cf5b)
