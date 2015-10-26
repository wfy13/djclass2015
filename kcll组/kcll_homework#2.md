# ---
#title: "TryR Codeschool exercise"
#date: "September 25th, 2015"
#group name: kcll
#---



############chapter1############
# tryR
#Expressions
1+1

"Arr, matey!"

6 * 7

#Logical Values
3 < 4

2 + 2 == 5

T == TRUE

#Variables
x <- 42
x / 2

x <- "Arr, matey!"
x

x <- TRUE

#Functions
sum(1, 3, 5)

rep("Yo ho!", times = 3)

sqrt(16)

#Help
help(sum)

example(min)

help(rep)

#Files
list.files()
source("bottle1.R")
source("bottle2.R")



###########chapter2############
# Vectors
#Vectors
c(4, 7, 9)

c('a', 'b', 'c')

c(1, TRUE, "three")

#Sequence Vectors
5:9

seq(5, 9)

seq(5, 9, 0.5)

9:5

#Vector Access
sentence <- c('walk', 'the', 'plank')
sentence[3]
sentence[1]
sentence[3] <- "dog"
sentence[4] <- 'to'
sentence[c(1, 3)]
sentence[2:4]
sentence[5:7] <- c('the', 'poop', 'deck')
sentence[6]

#Vector Names
ranks <- 1:3
names(ranks) <- c("first", "second", "third")
ranks
ranks["first"]

ranks["third"] <- 4

#Plotting One Vector
vesselsSunk <- c(4, 5, 1)
barplot(vesselsSunk)

names(vesselsSunk) <- c("England", "France", "Norway")
barplot(vesselsSunk)

barplot(1:100)

#Vector Math
a <- c(1, 2, 3)
a + 1

a / 2

a * 2

b <- c(4, 5, 6)
a + b
a - b

a == c(1, 99, 3)

a < c(1, 99, 3)

sin(a)
sqrt(a)

#Scatter Plots
x <- seq(1, 20, 0.1)

y <- sin(x)

plot(x, y)

values <- -10:10
absolutes <- abs(values)
plot(values, absolutes)

#NA Values
a <- c(1, 3, NA, 7, 9)
sum(a)
help(sum)
sum(a, na.rm = TRUE)



###########chapter3############
#Matrices
#Matrices
matrix(0,3,4)

a <- 1:12
print(a)

matrix(a, 3, 4)

plank <- 1:8
dim(plank) <- c(2, 4)
print(plank)

matrix(1, 5, 5)

#Matrix Access
print(plank)

plank[2, 3]

plank[1, 4]

plank[1, 4] <- 0

plank[2,]

plank[, 4]

plank[, 2:4]

#Matrix Plotting
elevation <- matrix(1, 10, 10)

elevation[4, 6] <- 0

contour(elevation)
persp(elevation)
persp(elevation, expand=0.2)
contour(volcano)
persp(volcano, expand=0.2)
image(volcano)




###########chapter4############
#Summary Statistics
#Mean
limbs <- c(4, 3, 4, 3, 2, 4, 4, 4)
names(limbs) <- c('One-Eye', 'Peg-Leg', 'Smitty', 'Hook', 'Scooter', 'Dan', 'Mikey', 'Blackbeard')
mean(limbs)
barplot(limbs)

abline(h = mean(limbs))

#Median
limbs <- c(4, 3, 4, 3, 2, 4, 4, 14)
names(limbs) <- c('One-Eye', 'Peg-Leg', 'Smitty', 'Hook', 'Scooter', 'Dan', 'Mikey', 'Davy Jones')
mean(limbs)

barplot(limbs)
abline(h = mean(limbs))

median(limbs)

abline(h = median(limbs))

#Standard Deviation
pounds <- c(45000, 50000, 35000, 40000, 35000, 45000, 10000, 15000)
barplot(pounds)
meanValue <- mean(pounds)
abline(h = meanValue)
deviation <- sd(pounds)
deviation

abline(h = meanValue + deviation)

abline(h = meanValue - deviation)

