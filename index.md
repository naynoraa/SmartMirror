# Smart Mirror
My project is the Smart Mirror, which displays various essential data like the time, weather, and current events through the use of Raspberry Pi and various coding languages like JavaScript, CSS, and Python. In addition to the default modules, I also added some modifications like adding animated icons for my weather module and an IR sensor to turn the Smart Mirror on if someone stands in from of it.

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Aaron Yan | Lynbrook High School | Engineering | Incoming Junior

![Headstone Image]
  
# Final Milestone

[![Final Milestone]

# Second Milestone: Adding Modifications

My second milestone was modifying my Smart Mirror even further by changing my weather icons into animated ones and adding an ultrasonic sensor in order to make my Smart Mirror turn on and off depending on whether someone is in front of it or not. In order to get my animated weather icons, I first had to download a package of them from the internet and put it in my css folder. From there, I added various blocks of cod eto my custom.css file, which complete the changing process. For my ultrasonic sensor, I first tried using python, a language I had never used before, and my terminal in order to open my Magic Mirror when someone was detected. However, this was very slow, so I tried searching online for a module that did the same thng and installed it into my code, but the installation didn't work for some reason. This brought me back to the python idea. This time, I decided to have both the MagicMirror Screen and a blank screen and switch between them using the terminal with the tvservice -p (turns monitor on), tvservice -o (turns monitor off), and chvt6 && chvt 7 (orients screen) commands.

![image](https://cdn.discordapp.com/attachments/869253167156711444/873238633195397190/ezgif-4-da96d34b3115.gif)

```css
.currentweather, .wi-day-sunny {
content: url("/css/icons/animated/day.svg");
}

.currentweather, .wi-day-cloudy {
content: url("/css/icons/animated/cloudy-day-1.svg");
}

.currentweather, .wi-rain {
content: url("/css/icons/animated/rainy-6.svg");
}

.currentweather, .wi-night-clear {
content: url("/css/icons/animated/night.svg");
}

.currentweather, .wi-night-cloudy {
content: url("/css/icons/animated/cloudy-night-2.svg")
}

.currentweather, .wi-cloudy {
content: url("/css/icons/animated/cloudy.svg");
}

.currentweather, .wi-showers {
content: url("/css/icons/animated/rainy-7.svg");
}

.currentweather, .wi-thunderstorm {
content: url("/css/icons/animated/thunder.svg");
}

.currentweather, .wi-snow {
content: url("/css/icons/animated/snowy-6.svg");
}

.currentweather, .wi-cloudy-windy {
content: url("/css/icons/animated/cloudy-day-3.svg");
}

.currentweather, .wi-night-rain {
content: url("/css/icons/animated/rainy-6.svg");
}

.currentweather, .wi-night-snow {
content: url("/css/icons/animated/snowy-6.svg");
}

.currentweather, .wi-night-thunderstorm {
content: url("/css/icons/animated/thunder.svg");
}

.currentweather, .wi-night-showers {
content: url("/css/icons/animated/rainy-7.svg");
}

.currentweather, .wi-fog {
content: url("/css/icons/animated/cloudy.svg");
}

.currentweather, .wi-night-alt-cloudy-windy {
content: url("/css/icons/animated/cloudy-night-1.svg");
}
```

Code that I used in order to change the weather icons into animated ones in the current weather section. Specifically, the code works by targetting certain icons in certain parts of my Smart Mirror, like the "wi-day-sunny" icon in the "currentweather" section. From there, it takes an icon I downloaded from the internet by entering into it's file and replaces the previous icon.

```css
.weatherforecast, .wi-day-sunny {
content: url("/css/icons/animated/day.svg");
  height: 48px;
  margin-top: 10px;
}

.weatherforecast, .wi-day-cloudy {
content: url("/css/icons/animated/cloudy-day-1.svg");
  height: 48px;
  margin-top: 10px;
}

.weatherforecast, .wi-rain {
content: url("/css/icons/animated/rainy-6.svg");
  height: 48px;
  margin-top: 10px;
}
```
Code that I used in order to change the weather icons into animated ones in the forecast section. The code here is mostly the same, but these have extra code to change their size with the "height" variable and their position with the "margin-top" variable, leading to a better-looking mdoule.

[![Third Milestone]
# First Milestone: Setting Up
  

My first milestone was setting up and hooking up the Raspberry Pi and all the necessary components onto my monitor and installing the Smart Mirror program. In order to get the Rasberry Pi working, I had to first download the corrosponding software and upload it onto a USB, which I then used plugged into my Raspberry Pi. From there, I connected a monitor and keyboard and mouse, allowing me to see and edit my smart mirror. Here, I ran into a few roadblocks, with the main one being getting used to the foreign UI and coding language used. Fortunately, I was able to figure it out and start working on my smart mirror!

<html><iframe width="560" height="315" src="https://www.youtube.com/embed/Sqnx8fd6HXA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></html>
