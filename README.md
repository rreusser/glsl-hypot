# glsl-hypot

> The 2D hypot function for GLSL

[![glsl-hypot](https://nodei.co/npm/glsl-hypot.png?mini=true)](https://nodei.co/npm/glsl-hypot)

## Introduction

`sqrt(x * x + y * y)` is easy, but it's subject to overflow. This function returns the length of a vec2 while avoiding overflow/underflow. Most of the time, you're almost certainly fine without this.

## Usage

``` glsl
#pragma glslify: hypot = require(glsl-hypot)

attribute vec3 position;

void main () {
  gl_FragColor = vec4(vec3(hypot(position.xy)), 1.0);
}
```

## License

&copy; 2016 Ricky Reusser. MIT License.
