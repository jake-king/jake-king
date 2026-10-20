# Jake King

I'm a software engineer in Ventura, CA. For the past ten years I was the sole developer on [TeachRock](https://teachrock.org/), a free K-12 curriculum site that about 80,000 teachers use. I built the site, and the analytics pipeline that showed the foundation how it was being used. Before that I spent seven years at Zinio making interactive digital editions of magazines like PC Magazine and Marie Claire.

Most of my free time goes into building things. I run a small NixOS homelab from a single repository, where coding agents can propose changes and I approve them. I'm also working on a CPU for a small FPGA board, a laptop shaped like an old ThinkPad X220, and a 2D game engine in Guile Scheme. I like knowing how things work at every layer, even the hardware.

I'm looking for my next role, ideally in platform or infrastructure work. If you're hiring, I'd be glad to hear from you on [LinkedIn](https://www.linkedin.com/in/jake-king-422789445).

## wasm_ascii_cam

[Demo](https://jake-king.github.io/wasm_ascii_cam/) · [source](https://github.com/jake-king/wasm_ascii_cam)

I started this in 2019 as a weekend experiment and recently came back to finish it properly. It turns a webcam or video file into coloured ASCII in the browser. The pixel conversion is Rust compiled to WebAssembly, split across Web Workers, with a SIMD path that's tested against the scalar code for every RGB value. Drawing is one WebGL2 draw call per frame using a glyph atlas; the Canvas 2D version it replaced took up to 73 ms a frame. You can also open a video file and export the result to WebM.

[![wasm_ascii_cam rendering a scene from Blender's Spring](https://raw.githubusercontent.com/jake-king/wasm_ascii_cam/master/docs/demo.gif)](https://jake-king.github.io/wasm_ascii_cam/)

<sub>Footage from <a href="https://studio.blender.org/films/spring/"><i>Spring</i></a>, © Blender Foundation, <a href="https://creativecommons.org/licenses/by/4.0/">CC BY 4.0</a>, converted to ASCII.</sub>
