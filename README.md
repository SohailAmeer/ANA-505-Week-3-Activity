# ANA-505-Week-3-Activity
Week 3 R Activity



getwd()
setwd()

women

womendata<-data.frame(women)
womendata

head(womendata,2)

nrow(womendata)
ncol(womendata)
colnames(womendata)
lapply(womendata,class)


summary(womendata)

mean(womendata$height)

womendata[,1]
womendata[,2]


df <- data.frame(womendata)


womendataindex <- df[(womendata$height>65),]
womendataindex


nrow(womendataindex)


ncol(womendataindex)


ncol(womendataindex) 
nrow(womendataindex)

  
install.packages("ggplot2")
  

library(ggplot2)


ggplot(womendata, aes(x=height, y=weight)) + 
  geom_point()

ggplot(womendata, aes(x=height, y=weight)) + 
  geom_point(shape = 21, colour = "black", fill = "white", size = 5, stroke = 5)
