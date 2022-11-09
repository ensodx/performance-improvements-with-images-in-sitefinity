# Performance improvements with images in Sitefinity
How to adapt the rendering of images to achieve 80-90% page size and performance reduction with Sitefinity. For more information, watch the [video here](https://www.instagram.com/reel/CkvMdDxgLza/?utm_source=github).


- [Summary](#Summary)
- [Installation](#Installation)
- [Usage](#Usage)
- [Credits](#Credits)
- [License](#License)
- [EnsoDX](#EnsoDX)

---
### Summary
---
This repository hosts an example approach towards 80-90% page size and performance improvements using a different approach to render images in Sitefinity.

On a sample page, with 2 full-width and 3 smaller images the total page size is reduced from 5.1Mb to 457Kb transfered.

The sample page includes some _lorem ipsum_ as content filler to allow for the additional bonus feature of all images being lazy loaded.

##### __Sitefinity 14.3 out of the box with Bootstrap 5 theme (page size: 5.1Mb).__
![alt text](https://raw.githubusercontent.com/ensodx/ensodx/8b7e331d37f1c96c588d6dc9327d622a58abc3df/assets/performance-improvements-with-images-in-sitefinity/screenshot-sitefinity-otb.png)

##### __Sitefinity 14.3 with Bootstrap 5 theme using the EnsoDX approach (page size: 457Kb).__
![alt text](https://raw.githubusercontent.com/ensodx/ensodx/8b7e331d37f1c96c588d6dc9327d622a58abc3df/assets/performance-improvements-with-images-in-sitefinity/screenshot-sitefinity-ensodx.png)


---
### Installation
---
This code assumes you have a working version of Sitefinity 14.3 running.

1. Clone the repository to your local system.
2. Replace your Sitefinity image widget view with the new view from this repository.
3. Add the thumbnail profiles from LibrariesConfig.config to your file.
3. Include the [javascript file](https://github.com/ivopetkov/responsively-lazy).
4. Include the [css file](https://github.com/ivopetkov/responsively-lazy).
5. You are ready to create your content.

> Be careful replacing files in an existing project as it will impact your solution and files

---
### Usage
---
The code should be used as reference and not directly copied into an existing system.

This implementation has a dependency on Ivo Petkov's library '[Responsively Lazy](https://github.com/ivopetkov/responsively-lazy)'

If you want to use this with existing image libraries, please ensure that the thumbnail profiles from step 3 of the installation, are selected for your libraries and thumbnails are regenerated.


---
### Credits
---
- [Ivo Petkov](https://github.com/ivopetkov/responsively-lazy)'s repository Responsively-Lazy.
- [Sabrie Nedzhip](https://www.linkedin.com/in/sabrie-nedzhip/) for writing the code.
- [Jochem Bökkers](https://www.linkedin.com/in/jbokkers/) for writing the sample and documentation.

---
### License
---
Free to use under the [MIT license](http://opensource.org/licenses/MIT).

Sitefinity is a registered trademark of [Progress Software Corporation](https://www.progress.com/sitefinity-cms).


---
### EnsoDX
---
Enso DX is a service provider company, specializing in scaling and digital experience transformation and migration projects. We focus on architecting, developing and streamlining the implementation for web and multi-channel projects by taking a holistic approach to ensure successful project implementations that align with your long term and sustainable strategic objectives.
