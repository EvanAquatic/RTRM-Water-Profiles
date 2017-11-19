library(ggplot2)

RTRM<- read.csv("~/###DATALOCATION", header=TRUE, na.strings = "NA")

df<-data.frame(RTRM)

g<-ggplot(df, aes(x=Water, y =Depth, color=Legend))+
  theme_bw() + 
  geom_path(aes(linetype=Legend), ) + 
  facet_wrap(~Month, ncol=5)+
  labs(title='Mean Water Temperature Profiles by Month in 2016') +
  xlab("Temperature (C)")+
  ylab("Depth (m)")+
  scale_y_reverse() +
  theme(strip.text = element_text(size=6.5, lineheight=0.1, hjust=0.5),
        axis.text.y = element_text(size=8),
        axis.text.x = element_text(size=8))
