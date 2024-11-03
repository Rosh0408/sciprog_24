# Practical2

This folder contains code for practical2 session

## Compile 
gcc Coversion.c Conversion -lm
gcc Sum.c Sum -lm

## Execute 

 ./Conversion

The number of digits is 25
inum=33554431,  fnum=33554432.000000, inum in binary=1111111111111111111111111

 ./Sum


 Sum1=7.485478
 Sum2=7.485472
 Difference between the two is 0.000007
 
 library(ggplot2)

# Sample data frame
set.seed(123)  # For reproducibility
df <- data.frame(
  group = factor(rep(c("A", "B", "C"), each = 100)),
  y = c(rnorm(100, mean = 5, sd = 1),
        rnorm(100, mean = 7, sd = 1.5),
        rnorm(100, mean = 6, sd = 1))
)

# Create the plot
ggplot(df, aes(x = group, y = y)) +
  geom_violin() +
  geom_dotplot(binaxis = "y", stackdir = "center", position = position_dodge(0.75), dotsize = 0.5) +
  labs(title = "Violin Plot with Dot Plot Overlay", x = "Group", y = "Y Value")
