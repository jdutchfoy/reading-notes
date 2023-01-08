# README.md

## Read assignment 11

One of the notable advancements in the audio sector since the 2000s is the introduction of digital streaming platforms. Websites like YouTube, MySpace, and Napster were part of the early group of companies that supported music streaming. They allowed artists to upload and share their music with a global audience for free. More recently, there have been other streaming sites like SoundCloud along with downloadable platforms like Spotify, TIDAL, and Apple Music.
2.In the same way as for the <img> element, the src (source) attribute contains a path to the  	video you want to embed. It works in exactly the same way.Users must be able to control video and audio playback (it's especially critical for people who have epilepsy.) You must either use the controls attribute to include the browser's own control interface, or build your interface using the appropriate JavaScript API. At a minimum, the interface must include a way to start and stop the media, and to adjust the volume.


3.The paragraph inside the <video> tags
This is called fallback content — this will be displayed if the browser accessing the page doesn't support the <video> element, allowing us to provide a fallback for older browsers. This can be anything you like; in this case, we've provided a direct link to the video file, so the user can at least access it some way regardless of what browser they are using.

4.CSS Grid Layout (aka “Grid” or “CSS Grid”), is a two-dimensional grid-based layout system that, compared to any web layout system of the past, completely changes the way we design user interfaces. CSS has always been used to layout our web pages, but it’s never done a very good job of it. First, we used tables, then floats, positioning and inline-block, but all of these methods were essentially hacks and left out a lot of important functionality (vertical centering, for instance). Flexbox is also a very great layout tool, but its one-directional flow has different use cases — and they actually work together quite well! Grid is the very first CSS module created specifically to solve the layout problems we’ve all been hacking our way around for as long as we’ve been making websites.

5.Grid Container
The element on which display: grid is applied. It’s the direct parent of all the grid items. In this example container is the grid container.

Grid Line
The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column.

Grid Item
The children (i.e. direct descendants) of the grid container. Here the item elements are grid items, but sub-item isn’t.

Grid Cell
The space between two adjacent row and two adjacent column grid lines. It’s a single “unit” of the grid. 

6.Responsive web design is important in modern day as this allows our websites to adapt to several screen sizes.
Images do not gracefully adapt to different screen sizes without some effort to get them to.	Having responsive images is important because it helps us deliver optimal file size, the right image for the right screen size, improves user experience and improves loading time.	Having various versions of your image is important for creating a responsive image.

7. The standard <img> element traditionally only lets you point the browser to a single source file. srcset defines the set of images we will allow the browser to choose between, and what size each image is. Each set of image information is separated from the previous one by a comma. sizes defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true

8.Both srcset and picture do approximately the same thing, but there is a subtle difference:
picture dictates what image the browser should use, whereas
srcset gives the browser a choice. A lot of things can be used to select this choice like viewport size, users preferences, network condition and so on. Hopefully in the future browsers would become smarter and smarter with selecting the appropriate image.
The support for srcset is pretty good and almost all current browsers more or less support it. Situation with a picture element is a little bit worse.

## Things I want to know more about

Flex and Grid