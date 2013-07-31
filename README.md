# Polymer Slider Example

## Live Demo
[http://dl.dropboxusercontent.com/u/695740/webaudio-slider/index.html](http://dl.dropboxusercontent.com/u/695740/webaudio-slider/index.html)

![](https://raw.github.com/ryoyakawai/webaudio-slider/master/images/screenshot.jpg)

## How to use
- load polymer.js
- link to webaudio-knob component

```
<script src="[PathTo]/polymer.js">
<link rel="import" href="[PathTo]/knob.html">
```

- insert `webaudio-slider` element

```
<webaudio-slider id="hoge02" class="hoge02" basesrc="images/fader-base03.jpg" knobsrc="images/fader-knob03.jpg" value="40" min="0" max="100" step="1" basewidth="76" baseheight="300" knobwidth="35" knobheight="50" ditchLength="230"></webaudio-slider>
```

- create imperatively

```
var slider = document.createElement('webaudio-slider');
```

- value can be changed by simply dragging up and down

## Attributes
### 'min'
**description**: min value of the slider  
**default**: `0`

### 'max'
**description**: max value of the slider  
**default**: `100`

### 'value'
**description**: value of the slider  
**default**: `0`

### 'step'
**description**: value change steps by moving mouse  
**default**: `1`

### 'basewidth'
**description**: width of slider's baseimage  
**default**: `0`

### 'baseheight'
**description**: height of slider's baseimage  
**default**: `0`

### 'knobwidth'
**description**: width of slider's knobimage  
**default**: `0`

### 'knobheight'
**description**: height of slider's knobimage  
**default**: `0`

### 'ditchLength'
**description**: lenght of slider's dithch. Please adjust this value when the knob is pushed out from baseimage.
**default**: `0`

### 'basesrc'
**description**: path to slider's base image resource (relative from where you are refering)  
**default**: `null`

### 'basesrc'
**description**: path to slider's base image resource (relative from where you are refering)  
**default**: `null`

## Events
### 'change'
**description**: 'change' event emitted everytime value changes

```
var slider = document.getElementsByTagName('[id name of your slider element]');
slider.addEventListener("change", function(){
  console.log(this.value);
});
```


## License

The Apache License Version 2.0

