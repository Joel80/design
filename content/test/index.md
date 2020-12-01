---
Title: Test
Description: Testsida
Template: test
Hidden: true
---

## Testsida

# Laddar in bilden som vanligt
![Leaf](%assets_url%/img/leaf_256x256.png)
# Laddar in bilden via Cimage
![Leaf](image/leaf_256x256.png?h=250&w=150&stretch)

![Leaf](image/leaf_256x256.png?h=250&w=150&crop-to-fit)

![Leaf](image/alexandre-brondino--bi8zhvPhVA-unsplash_cropped.jpg?width=50%)

## Beskärning

![Leaf](image/leaf_256x256.png?area=50,0,0,0)

![Leaf](image/leaf_256x256.png?area=0,50,0,0)

![Leaf](image/leaf_256x256.png?area=0,0,50,0)

![Leaf](image/leaf_256x256.png?area=0,0,0,50)

![Leaf](image/leaf_256x256.png?crop=50,50,100,100)

## Kvalité och filstorlek
![Leaf](image/alexandre-brondino--bi8zhvPhVA-unsplash_cropped.jpg?q=50)

## Filter
![Leaf](image/alexandre-brondino--bi8zhvPhVA-unsplash_cropped.jpg?width=50%&convolve=lighten)

![Leaf](image/alexandre-brondino--bi8zhvPhVA-unsplash_cropped.jpg?width=50%&convolve=darken)

![Leaf](image/alexandre-brondino--bi8zhvPhVA-unsplash_cropped.jpg?width=50%&blur)

![Leaf](image/alexandre-brondino--bi8zhvPhVA-unsplash_cropped.jpg?width=50%&f=grayscale)

![Leaf](image/alexandre-brondino--bi8zhvPhVA-unsplash_cropped.jpg?width=50%&f=brightness,50)

![Leaf](image/alexandre-brondino--bi8zhvPhVA-unsplash_cropped.jpg?width=50%&f=contrast,50)

![Leaf](image/alexandre-brondino--bi8zhvPhVA-unsplash_cropped.jpg?v)


## Responsiva bilder

### Vanliga sättet

<picture>
    <source media="(min-width: 668px)" srcset="assets/img/sheep.jpg, sheep@2x.jpg 2x">
    <source media="(min-width: 376px)" srcset="assets/img/sheep-small-landscape.jpg">
    <img src="sheep-small-portrait.jpg" class="assets/img/max-width" alt="sheep">
</picture>

### Cimage

<picture>
    <source media="(min-width: 668px)" srcset="image/sheep.jpg">
    <source media="(min-width: 376px)" srcset="image/sheep.jpg?w=667">
    <img src="image/sheep.jpg?w=375" alt="sheep">
</picture>


### Video
<div class="embed-container">
    <iframe src="https://www.youtube.com/embed/gCwjLPBqpa0" frameborder="0" allowfullscreen></iframe>
</div>
