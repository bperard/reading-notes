# Media

## Video and Audio Content

**Explain how the ability to use video and audio on the web has evolved since the early 2000s.**
The first influx of online videos and audio were made possible by proprietary plugin-based technologies like Flash and Silverlight. Both of these had security and accessibility issues, and are now obsolete, in favor of native HTML solutions <video> and <audio> elements and the availability of JavaScript APIs for controlling them.

**Describe the use of the src and controls attributes in the <video> element.**

- In the same way as for the <img> element, the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.
-  You must either use the controls attribute to include the browser's own control interface, or build your interface using the appropriate JavaScript API. At a minimum, the interface must include a way to start and stop the media, and to adjust the volume.

**Why is it important to have fallback content inside the <video> element?**
*Fallback content* will be displayed if the browser accessing the page doesn't support the <video> element, allowing us to provide a fallback for older browsers

**Write a very short story where <audio> and <video> are characters.**
When I wanted to add audio to my page I used the <audio> tag, and when I needed to include visual media to make a better presentation I used the <video> tag.

## Grid

**How does Grid layout differ from Flex?**
Grid is  a two-dimensional grid-based layout system, and flex is  one-directional flow.

**Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.**

- *Grid Container*: The element on which display: grid is applied. It’s the direct parent of all the grid items.
- *Grid Item*: The children (i.e. direct descendants) of the grid container.
- *Grid Line*: The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column.

## Responsive Images

**Besides making a site visually appealing across different screen sizes, why should developers make images responsive?**
Responsive images allow your site to adjust based on the device it is being viewed on, rather than having a single optimized size.

**Define the following <img> attributes srcset and sizes. Write an example of how they are used.**

- *srcset*: Defines the set of images we will allow the browser to choose between, and what size each image is. Each set of image information is separated from the previous one by a comma
- *sizes*: Defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true.

**How is srcset more helpful for responsive images than CSS or JavaScript?**
It allows a site to only load the correct image needed for the site, rather than preloading one image and then switching to a more optimized size.
