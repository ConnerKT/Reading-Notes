# Audio, Video, Images

This topic is important to me because I want to be able to add more dynamic features to my site.

## References

<https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content>.
<https://css-tricks.com/snippets/css/complete-guide-grid/>.
<https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images>.
Class 5 Review <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML>.

## Video and Audio Content

The **video** tag allows you to embed a video very easily.

You put a src attribute on the tag to source a video.

A controls attribute allows the user to include the browsers own control interface. Or build your own with JS.
Putting a p tag inside of the video tag allows you to have a fall back incase the user fails to load the video.

Formats like MP3, MP4, and WebM are called **container formats**. They define a struture in which the audio and/or video tracks that make up the media that is stored.

A **type** attribute is optional but its best to include it.
It contains the MIME type of the file and browsers can use the type to skip videos that can't load on the browser.

A **source** tag is used to source multiple video links with different formats so in case it isn't supported on one users page, it is on the other.

In order to support multiple browsers, its best to include different sources so the video is there for everyone.

Different video featues include:
1. width and height
2. autoplay
3. loop
4. muted
5. preload

The audio element is just like the video element, just works with small differences.

This doesn't support the width/height attributes.

Poster as well, since theres on visual item.

Accessibility for people who can't listen to the video. Video text tracks.

In order to do so we use the webvvt file format and the **track tag**.

WebVTT is a format for writing text files containing multiple strings of text along with metadata such as the time in the video at which each text should be displayed.

Cues are what the text strings are called.

the cues are:

1. Subtitles
2. Captions
3. timed descriptions

    WEBVTT

    1
    00:00:22.230 --> 00:00:24.606
    This is the first subtitle.

    2   
    00:00:30.739 --> 00:00:34.074
    This is the second.


Save it as a .vtt file. And then with the track element after the source elements.

    <video controls>
    <source src="example.mp4" type="video/mp4" />
    <source src="example.webm" type="video/webm" />
    <track kind="subtitles" src="subtitles_es.vtt" srclang="es" label="Spanish" />
    </video>

### Video and Audio Content Questions

1. We used to use flash and other plugins, but now its incorporated as a feature on html.
2. Source gives the video that is played, controls give the feature to control the video.
3. Incase someones browser is outdated and doesn't support the file type.
4. Audio is a person who doesn't like dressing out but video is a person who is very expressive and shows a lot.

## A Complete Guide To Grid

CSS Grid is a two-dimensional grid-based layout system, it changes the way we design user interfaces. 

**display:grid** allows you to define the cotainer element.
**grid-template-columns** and **grid-template-rows** allow us to set the column and row sizes.
And then you set the child elements with **grid-column** and **grid-row**.

Grid-Line : The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column.

Grid-Track : The space between two adjacent grid lines. You can think of them as the columns or rows of the grid.

Grid-Area : The total space surrounded by four grid lines. A grid area may be composed of any number of grid cells.

Grid-Item : The direct descendatnts of the grid container.

Grid-Cell : the between two adjacent row and two adjacent colum grid lines. A single unit.

### A Complete Guide To Grid

1. Grid is two-dimensional, and flex is one dimensional on two axises.
2.Grid container is the parent, grid item is the childern thats in the grid, and the grid lines are the lines between those items.

## Responsive Images

Responsive Images are images that work well on devices with widely differing screen sizes, resolutions and other features.

Two attributes we can use are **srcset and sizes**.

**srcset** defines the set of images we will allow the browser to choose between.

    <img
    srcset="elva-fairy-480w.jpg 480w, elva-fairy-800w.jpg 800w"
    sizes="(max-width: 600px) 480px,
         800px"
    src="elva-fairy-800w.jpg"
     alt="Elva dressed as a fairy" />

**sizes** defines a set of media conditions, and indicates what image size would be best to choose. Before each comma we write:
1. A media condition
2. A space
3. The width of the slot

### Resolution Switching

You can choose an appropriate resolution image by using srcset with x-descriptors and without sizes.

    <img
    srcset="elva-fairy-320w.jpg, elva-fairy-480w.jpg 1.5x, elva-fairy-640w.jpg 2x"
    src="elva-fairy-640w.jpg"
    alt="Elva dressed as a fairy" />

### Responsive Images Questions

1. For accessibility between different browsers and situations.
2. Src set sets the images we will allow the browser to choose between and we can declare when its chosen. Sizes is used to set the condtions of the image.
3. It sets the width conditions of the page and gives other photos we can use as well.

## Things I want to know more about

I want to know about responsive design overall.

I want to know more about the images and when I can apply this.
