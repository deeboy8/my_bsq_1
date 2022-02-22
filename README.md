# my_bsq

# my_bsq

## About
`my_bsq` -- finds and prints the biggest square on a map

## How to compile
Compile by running `make` in the root directory

## Synopsis
`my_bsq [map.txt]`

## Description
`my_bsq` finds the largest possible square on a board while avoiding obstacles. The board is represented by a file passed as the program’s argument, respecting those constraints:

- Its first line contains the number of lines on the board (and only that)
- "." (representing a free space) and "o" (representing an obstacle) are the only allowed characters for the other lines
- All the lines will be the same length (except the first one), and that length is at least 1
- The map will have at least one line
- Each line is terminated by `\n`.

The program prints the board, identifying the biggest square with '.' replaced by "X" to represent the largest square found.

## Map generation
To generate a new map, run:d
`perl map_generator.pl <num_rows> <num_cols> <density_of_obstacles> > <output_file.txt>`

## Implementation notes
This project is implemented with a dynamic programming approach.