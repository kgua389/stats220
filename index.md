# My meme


![my_ass](https://user-images.githubusercontent.com/101312088/157610233-e87f781b-6410-465a-91de-8087e84397d4.png)


library(magick)

background <- image_blank(width = 500,
                          height = 500,
                          color = "#000000") %>%
  image_annotate(text = "No comment",
                 color = "#FFFFFF",
                 size = 80,
                 font = "Impact",
                 gravity = "center")



rat <- image_read("https://4.img-dpreview.com/files/p/TS560x560~forums/61261730/541112ec39fb4719a48a7e1da29e4344") %>%
  image_scale(500)

rat_dog <- c(background, rat) %>% 
  image_append(stack=TRUE)

rat_dog

image_write(rat_dog, "my_assignemnt.png")

I created this meme because I highly dislike dogs of this breed. I am not a racist. Just this one breed of dog in particular, due to their face. 
