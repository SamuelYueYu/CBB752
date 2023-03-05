# CBB752
Programs for CBB 752 course
This is an inplementation of the Smith-Waterman algorithm, using the Blosum score matrix to determine similarity between amino acids. The input format goes as follows:

parser = argparse.ArgumentParser(description='Smith-Waterman Algorithm')
parser.add_argument('-i', '--input', help='input file', required=True)
parser.add_argument('-s', '--score', help='score file', required=True)
parser.add_argument('-o', '--opengap', help='open gap', required=False, default=-2)
parser.add_argument('-e', '--extgap', help='extension gap', required=False, default=-1)
args = parser.parse_args()

The program contains two major parts: first is to compute the similarity matrix and find the similarity score, and next is to write out the original sequences, the matrix itself, the score, and a trace back formulation of the sequence comparison.

sample-input1.txt and sample-input2.txt are examples of input sequences for comparison, and the output should resemble sample-output1.txt and sample-output2.txt, respectively. 
