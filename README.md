# How To Play Wiki Content

🚧🚧🚧🚧

Currently this repo is still under construction. You can follow these efforts on the [static site generator here](https://github.com/SoulSloth/how-to-play-wiki-generator) 

🚧🚧🚧🚧

howtoplay.wiki

This is the contents for howtoplay.wiki, a fast, simple, and accurate wiki with no ads, trackers, or twitch stream integration. 

# How to contribute
- Make pull requests to this repository with [.edn files](https://clojuredocs.org/clojure.edn) files in the relevant directories.
- Add screenshots and other media to `/optimusAssets/`.
- Fix inaccuracies, add missing information, improve existing pages

# Rules for contributors

0. How To Play Wiki aims to be a fast, simple, and accurate wiki. Any content within pull requests or currently on the site should be rejected or removed.
1. No plagiarized or copyrighted content is allowed.

## Assets

Image assets should all be in [webp format](https://developers.google.com/speed/webp/). You can convert webp images like [with the `cwebp` tool like so](https://developers.google.com/speed/webp/docs/cwebp):

```bash
# Convert a single file(PNG in this example) to webp
cwebp -q $QUALITY $FILE -resize $NEWX $NEWY -crop $X $Y $XOFFSET $YOFFSET -o ./$(basename $FILE .png).webp

#Convert a directory of png files to webp
for file in ./$DIR/*; do
    [ -f "$file" ] || continue
    cwebp -q 60 "$file" -resize $NEWX $NEWY -crop $X $Y $XOFFSET $YOFFSET-o ./$OUTDIR/$(basename "$file" .png).webp
done
```

# License

The contents of this repository is public domain. By submitting text, images, or any other form of media, you waive any pretense of ownership to it.
