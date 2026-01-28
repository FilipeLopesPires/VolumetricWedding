![banner](https://github.com/FilipeLopesPires/VolumetricWedding/blob/main/media/Banner_GaussianSplat.png)

# Volumetric Wedding

There are moments in life we want to freeze time and immortalize them in our memories. This is one of them for me. As a video and 3D enthusiast, I had our guests capture us young newlyweds in 360. Different cameras, no genlock, no studio, just raw excitement from the moment.

Back in 2022 when the pictures were taken, I couldn't even get a reconstruction done. Today, this is what I can get from open-source tech ([COLMAP](https://github.com/colmap/colmap) + [LichtFeld Studio](https://github.com/MrNeRF/LichtFeld-Studio) + [SuperSplat](https://github.com/playcanvas/supersplat)), on a fairly limited GPU (RTX 3070), and some holiday time spent fine-tuning training parameters.

You can explore it [here](https://arrival.space/filipelopespires) (published on [Arrival.Space](https://github.com/arrival-space)). I'm sure in the future we'll reach a point where you'll be able to enjoy our actual faces!

## Awards

Volumetric Wedding was submitted to [The Polys](https://thepolys.com/) - Immersive Awards [Splat of the Year](https://thepolys.com/sploty/) and became a semi-finalist for the 2025 edition.
If you would like to support my submission, upvote it [here](https://arrival.space/filipelopespires). You can check out all semi-finalists [here](https://arrival.space/sploty2025).

<img alt="The Polys Immersive Awards Splat of the Year Semi-finalist Laurel Dark Mode" src="https://github.com/FilipeLopesPires/VolumetricWedding/blob/main/media/SPLOTY-Seminfinalist.svg#gh-dark-mode-only" width="25%">
<img alt="The Polys Immersive Awards Splat of the Year Semi-finalist Laurel Light Mode" src="https://github.com/FilipeLopesPires/VolumetricWedding/blob/main/media/SPLOTY-Seminfinalist-dark.svg#gh-light-mode-only" width="25%">

## Contributions & Future Work

If you believe you could help me achieve better results out of this challenging dataset, do reach out! 
I'm sure plenty of gaussian splatting experts out there can do a better job than myself.

I'm available to give you access to the source images, camera pose data and current splat results - just ask!

Here's what's on my to-do list in the meantime:

Input Dataset:
- get missing pictures from guests
- test downscaling heavier / higher-res pictures
- figure out how to align missing perspectives in colmap

GSplat Generation:
- optimize Lichtfeld training parameters futher and leverage masks better
- process with higher performance GPU (Heh... I should probably update my setup)
- explore [Nerfstudio](https://github.com/nerfstudio-project/nerfstudio/), [Postshot](https://www.jawset.com/) and [OpenSplat](https://github.com/pierotofy/OpenSplat) as alternatives to Lichtfeld
- explore different reconstruction approaches such as leveraging Apple's latest [SHARP](https://github.com/apple/ml-sharp) approach to generate a splat per-image and then align them into a single splat scene

## Credits

Created by Filipe Lopes Pires.

Special thanks to the following folks that have made themselves available to help me in this project:
- [Dan Zeitman](https://github.com/dzeitman)
