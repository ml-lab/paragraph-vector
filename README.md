paragraph-vector
================

paragraph vector trained by negative sampling<br>
This project requires a template library for linear algebra: Eigen (http://eigen.tuxfamily.org/index.php?title=Main_Page).

An online demo is available at: http://www.logos.t.u-tokyo.ac.jp/~hassy/implementations/paragraph_vector/

*USAGE*<br>
1) modify a line in the Makefile to use Eigen<br>
EIGEN_LOCATION=$$HOME/local/eigen #Change this line

2) run the command "make"

3) train a model using your corpus which should have a paragraph (or document, sentence) in each line<br>
./paragraph_vector -input input.txt -output result

4) use the resulting files for your purpose<br>
result.bin<br>
result.pv: each line has a paragraph ID and real values of its vector representation<br>
result.wv: each line has a word and real values of its vector representation

\<Reference\><br>
Quoc Le, Tomas Mikolov. Distributed Representations of Sentences and Documents. 2014. Proceedings of the 31st International Conference on Machine Learning (ICML-14), pages 1188--1196.
