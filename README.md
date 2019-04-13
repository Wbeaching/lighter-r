
# LIGHTER-R #
LIGHTER-R is a tool to (near-) optimally implement a given 4 × 4 SBox in using a reversible logic library (with an associated cost metric). This is an extension of the tool LIGHTER ([original publication](https://tosc.iacr.org/index.php/ToSC/article/view/806), [archived version](https://eprint.iacr.org/2017/101), [source codes](http://jeremy.jean.free.fr/pub/fse2018_layer_implementations.tar.gz)), which only works for 4 × 4 SBoxes for ASIC and CPU (classical computing).

## How to use ##
  
  `./non-lin-search [-a] [-v] [-w] [-u] [-q]
                   [-l NUMBER] [-p NUMBER] [-r NUMBER]
                   [-i SBOX] [-o SBOX]
                   [-f FILE]`

    -a : Enable all gates and all implemented combinaisons of these gates
    -v : Verbose mode
    -u : Expand only [-i] function (identity function by default)
    -w : Write graphe in file
    
    -q : Enable all reversible gates

    -l <value> : Define an upper bound on the cost of the implementations generated
    -p <value> : Define the number of threads used
    -r <value> : Define an upper bound on the RAM used by the algorithm

    -i <function> : define start function
    -o <function> : define arrival function

    -f <file> : Define which logic library you want to use

See the "README-lighter" file (which is the original readme content for the vanilla LIGHTER) for more information.

