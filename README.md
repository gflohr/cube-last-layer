# Cube Last Layer

This all-in-one HTML file can be used to look up all algorithms needed to
solve a 3x3x3 Rubik's Cube with the CFOP method aka the Fridrich Method.

## Installation

There is no real installation required. Either clone the repository or
download a release, extract it to a location of your choice, and open
the file `index.html` in your browser.

## Usage

### Language

The "application" (well, umh, not really an application but t...) can
dynamically switch between the default language English and the alternative
language German.

If you want to add your own language, search the source code
for the strings "_en" and "-en", duplicate the corresponding line, and modify
it for your language.  If you want to share your translation with the
community, create a pull request or open an issue in order to get in touch
with the author.

### Method

The CFOP method can be be down in two ways.

Full OLL/PLL requires just two
steps. In step one, all pieces of the last layer are oriented correctly, so
that the upper face has just one color (Orient Last Layer or OLL). In step
two, all pieces of the last layer are brought to their correct location
(Permute Last Layer or PLL).

Alternatively, you can split OLL and PLL (or just one of them) into two
steps. That requires fewer algorithms to memorize but is, of course, slower.

The steps required are:

1. OLL
	1. EOLL (Edge Orientation of Last Layer)
	2. OCLL (Orient Corners of Lasat Layer)
2. PLL
	1. CPOLL (Corner Permutation of Last Layer)
	2. EPLL (Edge Permutation Last Layer)

You can switch between both methods, and your decision will be saved.

### Selecting an Algorithm

For almost all cases, you have multiple algorithms at your choice. Selecting
one will let you replay all turns of that algorithm in a
[cube animation](https://github.com/larspetrus/Roofpig) in the top-left
corner.

Your choice of algorithm will be remembered for your next session.

If you want to add an

## Why is this Better than Algorithm Collection XYZ?

There are two main advantages:

1. All algorithms are animated.
2. If your favourite algorithm requires a turn of the U layer, the animation automatically reflects the correct perspective whereas other lists contain awkward `y` turns.

## Bugs and Caveats

The code is terrible spaghetti code. The main reason is the author being too
lazy to give the project a proper structure after it had grown and evolved.

Some of its odd style is owed to the requirement that the HTML file should
work with plain `file://` URLs.

