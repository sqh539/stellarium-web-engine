Stellarium Web Engine（修改版）
==============================

> 本项目基于 [Stellarium Web Engine](https://github.com/Stellarium/stellarium-web-engine)（由 Stellarium Labs SRL 开发）修改发布，
> 依据 [GNU AGPL v3](LICENSE-AGPL-3.0.txt) 许可证开放源代码。
> 原项目版权归 Stellarium Labs SRL 所有。

About
-----

Stellarium Web Engine is a JavaScript planetarium renderer using
WebGL that can be embedded into a website.

Features
--------

- Atmosphere simulation.
- Gaia stars database access (more than 1 billion stars).
- HiPS surveys rendering.
- High resolution planet textures.
- Constellations.
- Support for adding layers and shapes in the sky view.
- Landscapes.


Build the javascript version
----------------------------

You need to make sure you have both emscripten and sconstruct installed.

    # Setup emscripten path.
    source $PATH_TO_EMSDK/emsdk_env.sh

    # Build stellarium-web-engine.js and stellarium-web-engine.wasm
    # This will also copy the files into html/static/js
    make js

    # Now see apps/simple-html/ to try the library in a browser.


Contributing
------------

In order for your contribution to Stellarium Web Engine to be accepted, you have to sign the
[Stellarium Web Contributor License Agreement (CLA)](doc/cla/sign-cla.md).
