# Practicing reprex

library(tidyverse)
library(palmerpenguins)


## NOT A REPREX

penguins |> 
  select(species, body_mass_g, flipper_length_mm, year) |> 
  filter(species == "Chinstrap") |> 
  str_to_lower(species) |> 
  group_by(islands) |> 
  summarize(mean(body_mass_g, na.rm = TRUE),
            mean(flipper_length_mm, na.rm =TRUE))

### A reprex version

library(tidyverse)

warpbreaks |> 
  mutate(wool = str_to_lower(wool))

### A reprex with a synthesized data frame

library(tidyverse)

data_frame <- tribble(
  ~letter, ~number,
  "A", 1,
  "B", 2,
  "C", 3
)

data_frame |> 
  mutate(letter = str_to_lower(letter))
