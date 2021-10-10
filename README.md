# [demo] Image Optimization

This demo shows the importance of optimizing images. 

## Things to note:

"The foundation of the whole internet is data compression"

## Image Types:
- JPEG/JPG: 
  - lossy image (doesn't need to store information such as location, camera, etc.) 
  - creates a small file size, should be used when you have full colour background (no transparencies). 

- PNG
  - lossless image (stores somme information).
  - creates a larger filesize than jpgs by default.
  - should only be used when transparencys are need.
  
  
- GIF
  - For animated or really small file sizez (8-bit/16-bit)
  - such as memes or really small icons.
  - P.S. we have better options now! 


See here for more details on image formats: https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization#selecting_the_right_image_format![image](https://user-images.githubusercontent.com/5560529/136681920-a4ff3f7d-e808-43fc-b7e6-15914019ac2f.png)


## Better Formats for the web!!

- SVG
  - SVG stands for Scable Vector Graphics. 
  - SVGs are great because we can make them as small or large as we need and the quality is never compromised (not pixel-based). 
  - SVGs are created using XML code and are relative small files, and can be used on your websites in 3 ways. 
    - as an HTML Image ```html <img src="icon.svg" alt="svg"/> ```
    - CSS background image  
    - Inline SVG - svg is also a markup language.

- WebP
  - NEW Gen Format of images for the web. This format was created for web images.
  - It compresses ~30% more than jpgs/jpegs and pngs.
  - It's supported in almost all browsers (Not in E11 and down), support is getting better. See [Can I Use](caniuse.com) for more info. 
    - As a note, where webp doesn't work in certain browsers we have other elements that allow for fallback images using the ```html <picture> ``` which we will be looking later in the course. Just to note that the format exists. 

## In This course:
The images you will use will primarily be:
- Webp (better than jpg)
- JPG/JPEG
- PNG
- SVG

## Steps to resizing images:

- Using Photoshop:
1. Determine your image ratio (larger # / smaller #) = ratio
2. Resize images to the largest size they will be rendered as
3. Save images with the proper format and reduced/optimized quality. In Photoshop this is best done by -> 'Export -> Save for Web (Legacy)' or using 'Export As'
4. Lastly, run the image through a third party compression tool

- Using Squoosh.app:
  - can resize images within the tool and as a side by side comparison it did a better job than Pho-toshop for compression.
 
 ### Compression Tools:
 
  - Imagemin (run as a dependancy)
  - Kraken.io
  - TinyPNG.com
  - ImageOptim (Mac app)
  - https://squoosh.app/ (Online drop and drag tool)

See more here: https://themeisle.com/blog/best-online-image-optimizer-tools/

Further reading: https://web.dev/fast/#optimize-your-images 


