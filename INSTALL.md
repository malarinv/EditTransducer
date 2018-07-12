### Installation Instructions :

#### macOS (Tested on 10.11.6)

-   `brew install -v https://github.com/malarinv/homebrew-science/raw/master/Formula/openfst.rb`
-   `brew install -v re2`
-   `pipenv install --skip-lock http://www.opengrm.org/twiki/pub/GRM/PyniniDownload/pynini-1.9.1.tar.gz`
-   `pipenv install --skip-lock https://github.com/malarinv/EditTransducer/archive/master.zip`

#### Linux (Tested on Centos 7)

-   `wget http://www.openfst.org/twiki/pub/FST/FstDownload/openfst-1.6.7.tar.gz`
-   `tar -xzvf openfst-1.6.7.tar.gz;cd openfst-1.6.7`

-   build and install
-     ./configure --prefix=/usr \
                  --disable-dependency-tracking \
                  --enable-compact-fsts \
                  --enable-compress \
                  --enable-compress \
                  --enable-const-fsts \
                  --enable-far \
                  --enable-linear-fsts \
                  --enable-lookahead-fsts \
                  --enable-mpdt \
                  --enable-ngram-fsts \
                  --enable-pdt \
                  --enable-special
      make -j4 && make install
-   `sudo yum install -y re2-devel`
-   `pipenv install --skip-lock http://www.opengrm.org/twiki/pub/GRM/PyniniDownload/pynini-1.9.1.tar.gz`
-   `pipenv install --skip-lock https://github.com/malarinv/EditTransducer/archive/master.zip`
