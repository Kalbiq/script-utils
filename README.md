# script-utils
Scripts that I wrote for my convenience. Feel free to use them.

### get-unsplash
This script downloads all images from links given in a file. They are downloaded in their original size. When calling the script you should include path to file with links as first argument and an existing directory path to save the images to as the second argument. Remember to make a new blank line at the bottom of the links file, otherwise the last link won't be downloaded.

##### Example use:
links.txt:
```
1.  https://unsplash.com/photos/LX_NkGTwHpo
2.  https://unsplash.com/photos/URi_yR9qtgs
3.  
```
(don't include the line numbers)

In terminal:
```
get-unsplash Desktop/links.txt Downloads/
```

Downloads folder:
```
LX_NkGTwHpo.jpg
URi_yR9qtgs.jpg
```

### meteo-pl
This scripts downloads the latest weather report graph from [meteo.pl](https://www.meteo.pl/) for the given town (for now in Poland). After it finishes the download it will open it in your default image viewer.
To get the list of available cities use ```meteo-pl -h```.
By default the image is downloaded to your Downloads folder, but it can be easily changed in the script file.
If you don't know how to read the graph then go to [meteo.pl](https://www.meteo.pl/) and select the report for any city, there will be a legend near the graph.

It should look like this, although they might change something:
![legend](https://www.meteo.pl/um/metco/leg_um_en_cbase_256.png "Graph legend")

##### Example use:
In terminal:
```
meteo-pl poznan
```