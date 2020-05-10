# Astraea

The planet generator inspired by [Planetarium](https://managore.itch.io/planetarium). Please see also [Twitter bot](https://twitter.com/astraea_yk).

![](https://user-images.githubusercontent.com/59264002/81490997-a30c6d00-92c3-11ea-8263-d79388ff2dd6.png)

## Algorithm

By shaving off the extra pixels from the square and bringing them together in the center, the 2D sprite is made to look like 3D.

![](https://user-images.githubusercontent.com/59264002/81490999-a6075d80-92c3-11ea-999c-99a6f06e76b3.png)

The planets' patterns are generated by some simple noise functions.  
If the plane references 2D noise, it will be scaled incorrectly, like Mercator projection. Therefore, the 3D noise is compressed into a 2D plane.  
In other words, it converts 3D noise into a 2D plane and makes it look like a 3D sphere.

![](https://user-images.githubusercontent.com/59264002/81491000-a7d12100-92c3-11ea-9a43-158e6d914f3e.png)

Please see my blog [post](https://yurkth.hateblo.jp/entry/astraea-planet-generator) for more information (sorry, it's Japanese).

## License

Astraea is licensed under the MIT license. See the [LICENSE](https://github.com/yurkth/astraea/blob/master/LICENSE) for more information.

### Libraries

- [p5.js](https://github.com/processing/p5.js) is licensed under the LGPL-2.1 license.
- [seedrandom](https://github.com/davidbau/seedrandom) is licensed under the MIT license.
- [simplex-noise](https://github.com/jwagner/simplex-noise.js) is licensed under the MIT license.
- [poisson-disk-sampling](https://github.com/kchapelier/poisson-disk-sampling) is licensed under the MIT license.
- [zlib.js](https://github.com/imaya/zlib.js) is licensed under the MIT license.

### Assets

- The [Corpora](https://github.com/dariusk/corpora) is licensed under the CC-0 license.
- The [PICO-8 font](https://www.lexaloffle.com/bbs/?tid=3760) (unofficial) does not claim any copyright.
  - The [official font](https://www.lexaloffle.com/pico-8.php?page=faq) is also licensed under the CC-0 license.

### References

- [TIC-80](https://github.com/nesbox/TIC-80) is licensed under the MIT license.
  - To draw a circle in pixels, I used the [circb](https://github.com/nesbox/TIC-80/blob/master/src/tic.c#L948-L961) function as a reference.

