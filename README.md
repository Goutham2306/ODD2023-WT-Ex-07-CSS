# Ex-07-CSS
## AIM:
Using CSS media queries, modify the webpage's color scheme with the following requirements: Default Color Scheme: Background color: Light gray (#f4f4f4) Text color: Dark gray (#333) Link color: Blue (#007bff) Small Screen Adaptation (Max-width: 600px):

## Objective 1:
Using CSS media queries to modify the webpage's color scheme.
## Step-1:
The HTML document starts with the usual declaration.The tag specifies the language as English (lang="en").The section includes meta tags for character set and viewport settings. The title of the webpage is set to "Color Scheme."

## Step-2:
The default color scheme for the webpage is defined in the body and a (anchor) styles. The background color is set to a light gray (#f4f4f4), text color is set to dark gray (#333), and anchor links are set to a blue color (#007bff).

## Step-3:
A media query is used to adjust the color scheme for small screens (max-width: 600px).On small screens, the background becomes dark (#333), text color becomes light (#f4f4f4), and anchor links turn green (#28a745).Media Query for Dark Mode Preference:

## Step-4
Another media query is used to check if the user prefers a dark color scheme.In dark mode, the background becomes black (#000), text color becomes white (#fff), and anchor links turn a teal color (#17a2b8).

## Step-5:
The section contains two heading elements and an anchor link .The headings are for displaying information, and the anchor link is an example to demonstrate the color change on different screen sizes and preferences.

## Step-6:
Testing: You can test the behavior by resizing the browser window to see the color scheme changes for small screens.If your system has dark mode preference enabled, the dark color scheme should be applied.

## CODE:
```
<html>
<!DOCTYPE.html>
<head>
</head>
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

<body>
<p>Welcome to Goutham's Webpage</p>
<a href="saveetha.ac.in">SAVEETHA WEBSITE</a>
</body>
</html>
```
## OUTPUT:
# If the user set the device in Light Mode:
![Screenshot 2023-12-15 054742](https://github.com/Goutham2306/ODD2023-WT-Ex-07-CSS/assets/138971154/33ed20ca-f18f-4f50-b103-7a06ca5461fb)

# If the user set the device in Dark Mode:
![Screenshot 2023-12-15 054612](https://github.com/Goutham2306/ODD2023-WT-Ex-07-CSS/assets/138971154/3a0b7eb1-b8dd-4c2a-aefe-cf1a9e3b60b2)

## Objective 2:
# Using CSS media queries to modify mobile and desktop styles.
## Step-1:
HTML Structure: The HTML document starts with the usual declaration.The tag specifies the language as English (lang="en").The section includes meta tags for character set and viewport settings. The title of the webpage is set to "Color Scheme."

## Step-2:
CSS Styles: The CSS styles are defined inside a <style> tag in the section.Styles for desktop devices are defined initially, setting the font size, background color, and text color for the body. A container class is defined for styling a central content container with a maximum width, padding, background color, border, and box shadow.Class selectors like .container, .device-specific, and .device-specific2 are used to target specific HTML elements for styling.

## Step-3:
Media Query for Mobile Devices: A media query (@media screen and (max-width: 599px)) is used to apply different styles for mobile devices with a width less than 600px.Inside the media query, the font size, background color, and text color for the body are adjusted for smaller screens.The styles for the .container class are modified, reducing padding, changing the background color, removing the box shadow, and adjusting the border.Two additional classes, .device-specific and .device-specific2, are defined with specific styles (bold and different colors) to demonstrate how styles can be tailored for mobile devices.

## Step-4:
To observe the responsive design, you can resize the browser window or use a developer tool to simulate different device widths.Notice how the styles change when the screen width is less than 600px, reflecting a mobile-friendly design.

## Step-5:
Testing: To observe the responsive design, you can resize the browser window or use a developer tool to simulate different device widths.Notice how the styles change when the screen width is less than 600px, reflecting a mobile-friendly design.

## CODE:
```
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
  <title>Media Queries 2</title>
</head>
<body>
  <div class="container">
    <h1>Responsive Blog Post</h1>
    <p>This is Goutham from Tirupati</p>
    <p class="device-specific">Important information is highlighted with bold text and a different color on mobile devices.</p>
  </div>
</body>
</html>
```
## OUTPUT:
# If the user was using the large screens like laptops,pc's:

![Screenshot 2023-12-15 054953](https://github.com/Goutham2306/ODD2023-WT-Ex-07-CSS/assets/138971154/c49fcc97-70a2-45bc-a0b8-b09c05f3545a)

# If the user was using the small screens like mobile:

![WhatsApp Image 2023-12-15 at 05 52 02_e7cb5672](https://github.com/Goutham2306/ODD2023-WT-Ex-07-CSS/assets/138971154/3e9d13a0-87d5-4d16-9141-e75e6d7794f3)

## Ojective 3:
# Using CSS media queries to represent orientation scheme.
## Step-1:
The HTML document starts with the usual declaration.The tag specifies the language as English (lang="en").The section includes meta tags for character set and viewport settings. The title of the webpage is set to "Color Scheme."

# Step-2:
CSS Styles: The CSS styles are defined inside a <style> tag in the section.Two media queries (@media (orientation: portrait) and @media (orientation: landscape)) are used to apply different styles based on the orientation of the device.

# Step-3:
Portrait Orientation Styles: Inside the @media (orientation: portrait) query, the background color of the body is set to a light blue (#e6f7ff). This will be applied when the device is in portrait orientation. Landscape Orientation Styles: Inside the @media (orientation: landscape) query, the background color of the body is set to a light purple (rebeccapurple). This will be applied when the device is in landscape orientation.

# Step-4:
Orientation Media Queries: The orientation media query is used to check whether the device is in portrait or landscape orientation.When the device is in portrait mode, the styles within @media (orientation: portrait) are applied.When the device is in landscape mode, the styles within @media (orientation: landscape) are applied.

Step-5:
Testing: To observe the changes based on orientation, you can view the webpage on a device with the capability to change orientations (such as a smartphone or tablet) or use a browser's developer tools to simulate different orientations.

## CODE:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Media Queries 3</title>
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
        background-color: rebeccapurple; /* Deep purple background for landscape orientation */
      }
    }
  </style>
</head>
<body>
  <h1>Webpage orientation using css media queries</h1>
  <p>Welcome to world of CSS</p>
  <p>this webpage is visible in purple colour on laptop and in light green when opened on smart phone</p>
</body>
</html>
```



