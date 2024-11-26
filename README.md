# R-Scripts


# Função Personalizada: Se você precisar repetir esse padrão várias vezes, pode transformá-lo em uma função:

install_and_load <- function(pkg) {
  if (!require(pkg, character.only = TRUE)) {
    install.packages(pkg, dependencies = TRUE)
    library(pkg, character.only = TRUE)
  }
}

# Exemplo de uso:
install_and_load("ggplot2")
install_and_load("dplyr")
