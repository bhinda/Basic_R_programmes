# Basic_R_programmes
# Numeric Factors
 
# First, as a vector
workshop <- c(1, 2, 1, 2, 1, 2, 1, 2)
workshop
table(workshop)
mean(workshop)
gender[workshop == 2]

# As a factor
workshop <- c(1, 2, 1, 2, 1, 2, 1, 2)
workshop <- factor(workshop)
workshop
table(workshop)
mean(workshop) #generates error now.
gender[workshop == 2]
gender[workshop == "2"]
 
# Recreating workshop making it a factor
workshop <- c(1, 2, 1, 2, 1, 2, 1, 2)
workshop <- factor(
workshop,
levels = c( 1,   2,     3,      4),
labels = c("R", "SAS", "SPSS", "Stata")
)
 
# Recreating it with just the levels 
workshop <- c(1, 2, 1, 2, 1, 2, 1, 2)
workshop <- factor(
workshop,
levels = c( 1,  2),
labels = c("R","SAS")
)
 
workshop
table(workshop)
gender[workshop == 2]
gender[workshop == "2"]
gender[workshop == "S"]
