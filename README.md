# Jupyter notebooks to create a realization of the "Singularity" video.

- To see the resulting video with the default configuration, check: https://vimeo.com/255980416

The data used to generate the video comes from the infrared "Wide-field Infrared Survey Explorer" (WISE) telescope [https://wise.ssl.berkeley.edu], and the base images processed are centred in the brightest galaxies contained in the redMaPPer v6.3 cluster catalogue [http://risa.stanford.edu/redmapper], which contains more than 20.000 clusters of galaxies. In the original satellite images, which can be seen almost unprocessed in the first ~10 seconds of the animation, each cluster member galaxy can be identified as a blob of light, meanwhile the forefront Milky Way stars are recognizable by their characteristic diffraction peaks. Some traces left by local meteors can be seen in the video too.

The images that compose the "Singularity" videos are produced only with the help of numerical codes commonly employed to process astrophysical images (python's `numpy`, `scipy` and `astropy` libraries). Apart from the "ffmpeg" open-source library, which is exclusively used to join the individually-generated frames into a video, no image or video processing software is used at all. 

The image effects sequence is designed to follow the amplitude and the pitch of the sound wave features of an input audio file. These effects are obtained processing and mixing each cluster image after applying different masks to both the real-space and the Fourier-space versions of the images. 

Each time the code runs, a random realization of the order and the amplitude of the sequence of cluster images is generated, so a different video is created each time too. The one linked above is the 4th realization of a series of 10, and hence the title of the video.

The sound I employed in my version was created using the "Sonic-Pi" open-source code [https://sonic-pi.net/] written by Sam Aaron. To create your own version of the video, input a different audio file and change the effects-sequence inside the code. For more in-depth changes or to create your own effects, check the code contained in the "python_libs" folder.

Pablo Jimeno.

©2018

PD: At the moment and due to the policies of some videoart festivals to which I submitted this work, the video cannot be public, so in case you want to check the resulting "Singularity #4" video linked above, contact me to obtain the password.
