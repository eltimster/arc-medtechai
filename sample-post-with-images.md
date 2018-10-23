---
layout: post
title:  "Sample Post with Images"
date:   2017-12-01 23:55:23 +1000
categories: []
---

## Add a video
```
{{ "{% include youtube_embed.html id='6EVs0BrG57I' " %}}}
```
{% include youtube_embed.html id='6EVs0BrG57I' %}

## Different sizes
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-xsmall post-block"}
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-xsmall post-block"}
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-small post-block"}
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-small post-block"}
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-medium post-block"}
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-medium post-block"}
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-large post-block"}
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-large post-block"}

## One photo by itself and centered
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-medium post-block"}
```
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-medium post-block"}

## Multiple photos in a line and centered
```
<span style="display:block;text-align:center">
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-medium post-inline"}
![Official Agreement Signing Photo](/assets/signing2017/002.jpg){:class="post post-medium post-inline"}
</span>
```
<span style="display:block;text-align:center">
![Official Agreement Signing Photo](/assets/signing2017/001.jpg){:class="post post-medium post-inline"}
![Official Agreement Signing Photo](/assets/signing2017/002.jpg){:class="post post-medium post-inline"}
</span>

## Single photo with caption
Parts to edit:
* file: path directory of the image
* class: follows the class details in the "Different sizes" section
* caption: description below the photo

```
{{'{% include image-with-caption.html file="/assets/signing2017/001.jpg" class="post post-medium post-block"
caption="Signing and looking at the camera" '}}%}
```
{% include image-with-caption.html file="/assets/signing2017/001.jpg" class="post post-medium post-block"
caption="Signing and looking at the camera" %}
## Multiple photos with caption in a line
Parts to edit:
* file: path directory of the image
* class: follows the class details in the “Different sizes” section
* caption: description below the photo

```
<div style="display:block;text-align:center">
{{'{% include image-with-caption.html file="/assets/signing2017/001.jpg" class="post post-medium post-inline"
caption="Signing and looking at the camera" '}}%}
{{'{% include image-with-caption.html file="/assets/signing2017/001.jpg" class="post post-medium post-inline"
caption="Signing and looking at each other" '}}%}
</div>
```
<div style="display:block;text-align:center">
{% include image-with-caption.html file="/assets/signing2017/001.jpg" class="post post-medium post-inline"
caption="Signing and looking at the camera" %}
{% include image-with-caption.html file="/assets/signing2017/002.jpg" class="post post-medium post-inline"
caption="Signing and looking at each other" %}
</div>
