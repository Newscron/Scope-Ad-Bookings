# Maxi Banners
* Only require/support `img` and`click`.

# ContentAd Style Ads
* Layout is either `image` or `textanzeige` or `topstory`
* `image` represents a pure image-ad, no text.
* `textanzeige` depends on the template: It could be a two column layout where we really show a picture, or just the text and the image is a 1x1 tracking pixel.
* `topstory` is an add that looks very similar to a regular article (of some chosen rendering style, but has a visual marker that indicates that this is an ad)
* Further relevant values: `title`, `text`, `linktext`, `click` (target URL), `img` (an image that is really shown, or just a tracking pixel).
* `display_title` is a DFV legacy field that we ignore.
* `bformat` is a DFV legacy field that we ignore.


# Client Specific Details
## KUHNFV1832
* The system supports one `topstory`
* `ContentAd-1` is the only ad slot that could be a `topstory`
* Rules: The "ContentAds" will appear in order after each article list. Exception: If the 1st slot is a top story, the top story will be printed as the first item, before any other editor element.