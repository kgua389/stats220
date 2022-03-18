**# My meme**

### I created this meme because I highly dislike dogs of this breed. I am not a racist. Just this one breed of dog in particular, due to their face and overly aggressive high pitched barks for no reason. To where I've got the inspiration and idea I would give credit to my neighbours dog.

![epic meme](https://user-images.githubusercontent.com/101312088/157612295-37c9617d-01c6-413c-98aa-8c557c6825a8.png)

```
library(magick)

background <- image_blank(width = 500,
                          height = 500,
                          color = "#000000") %>%
  image_annotate(text = "Yes I am a rat\n How did you know?",
                 color = "#FFFFFF",
                 size = 60,
                 font = "Impact",
                 gravity = "center")



rat <- image_read("https://4.img-dpreview.com/files/p/TS560x560~forums/61261730/541112ec39fb4719a48a7e1da29e4344") %>%
  image_scale(500)

rat_dog <- c(background, rat) %>% 
  image_append(stack=TRUE)

rat_dog

image_write(rat_dog, "my_assignment.png")
```
