---
layout: post
title: RSE2107A-Systems Engineering Project 1
description:  Design and create a physical arena inspired by a designated site at Changi Airport, ensuring it allows a 4-wheeled LIMO robot to perform key functions like localization, mapping, path planning, navigation, and obstacle avoidance. The robot will then navigate through multiple different other Arenas.
skills: 
  RTAB-Map Navigation 
  LIMO Robot Configuration 
  Arena Layout Design
main-image: /limo.png
---

---
# Project Requirement
To design and create a physical environment based on Changi Airport terminal 2, where a 4-wheeled mobile robot, i.e. LIMO robot from AgileX Robotics, is able to perform certain functions, localisation, mapping, path planning, navigation.


## Learning Outcomes  
- To be able to design and create a physical environment, i.e. a built environment or an
arena, where a mobile robot is able to move around.
- To be able to appreciate the tradeoff inherent in any real-world project and come up with
the best compromise.
- To be able to use the limo robot to navigate through the maze

## Arena 
Our design revolves around implied boundaries over solid walls to maintain the open aesthetic of Changi Airport Terminal 2. Instead of enclosed barriers, spaced obstacles like benches, pillars, or kiosks act as navigational cues, allowing the robot to interpret gaps as virtual walls while maintaining an open, human-friendly environment. This approach mirrors Changi’s balance of functionality and beauty, blending natural and architectural elements to create a visually appealing yet navigable space.

{% include image-gallery.html images="Arena.png" height="400" %}
---

---
## LIMO Robot Navigation

### RTAB-Map Implementation:
Configured RTAB-Map (Real-Time Appearance-Based Mapping) on ROS Noetic to create high-fidelity 2D/3D maps of dynamic arenas using a LIDAR and depth camera.
-Optimized parameters for loop closure detection to improve map accuracy in feature-sparse environments.
-Overcame "ghost walls" in the map by tuning Rtabmap db file

### Autonomous Navigation:
Developed a Python ROS script to
-Load pre-saved RTAB-Maps of each arena.
-Navigate through Arenas prompted by the user

Documentation of our approach can be seen in the document: 
---
---
[Full Documentation](https://docs.google.com/document/d/e/2PACX-1vSa_YLsK6IN35FtlLjiFyWISixE5j-9bfPvw5vEOq1qM6hP3iaN6D1vqKvEohXfWr9TFu_KwYFmEwf9/pub)



<!-- ### Header 3 
Use this to have subsection if needed
## Adding external links
[Full Documentation](https://docs.google.com/document/d/1bn3_BbAwyuse3n4ZvTmV1Wqgdn0dt24oMvfh_bcjxEo/edit?usp=sharing)

## Embedding images 
### External images
{% include image-gallery.html images="https://live.staticflickr.com/65535/52821641477_d397e56bc4_k.jpg, https://live.staticflickr.com/65535/52822650673_f074b20d90_k.jpg" height="400"%}
<span style="font-size: 10px">"Starship Test Flight Mission" from https://www.flickr.com/photos/spacex/52821641477/</span>  
You can put in multiple entries. All images will be at a fixed height in the same row. With smaller window, they will switch to columns.  

### Embeed images
{% include image-gallery.html images="project2.jpg" height="400" %} 
place the images in project folder/images then update the file path.   


## Embedding youtube video
The second video has the autoplay on. copy and paste the 11-digit id found in the url link. <br>
*Example* : https://www.youtube.com/watch?v={**MhVw-MHGv4s**}&ab_channel=engineerguy
{% include youtube-video.html id="MhVw-MHGv4s" autoplay= "false"%}
{% include youtube-video.html id="XGC31lmdS6s" autoplay = "true" %}

you can also set up custom size by specifying the width (the aspect ratio has been set to 16/9). The default size is 560 pixels x 315 pixels.  

The width of the video below. Regardless of initial width, all the videos is responsive and will fit within the smaller screen.
{% include youtube-video.html id="tGCdLEQzde0" autoplay = "false" width= "900px" %}  

<br>

## Adding a hozontal line
---

## Starting a new line
leave two spaces "  " at the end or enter <br>

## Adding bold text
this is how you input **bold text**

## Adding italic text
Italicized text is the *cat's meow*.

## Adding ordered list
1. First item
2. Second item
3. Third item
4. Fourth item

## Adding unordered list
- First item
- Second item
- Third item
- Fourth item

## Adding code block
```ruby
def hello_world
  puts "Hello, World!"
end
```

```python
def start()
  print("time to start!")
```

```javascript
let x = 1;
if (x === 1) {
  let x = 2;
  console.log(x);
}
console.log(x);

```

## Adding external links
[Wikipedia](https://en.wikipedia.org)


## Adding block quote
> A blockquote would look great if you need to highlight something


## Adding table 

| Header 1 | Header 2 |
|----------|----------|
| Row 1, Col 1 | Row 1, Col 2 |
| Row 2, Col 1 | Row 2, Col 2 |

make sure to leave aline betwen the table and the header

-->
