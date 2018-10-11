
# 서울대-삼성 DS<sup>2</sup> 기계학습 과정 실습 자료실

## 자료 다운로드 (**github 초보자 대상**)
  1. 화면 우측 상단의 녹색 'Clone or download' 버튼 클릭
  2. Download ZIP 클릭
  3. s2-ds2-master.zip 파일 압축 해제
  4. 압축 해제한 's2-ds2' 폴더를 '내 PC > 문서' 경로로 이동

  * *이후 상세한 설명은 상단 리스트의 실습환경_설치_가이드.pdf 참조*


---------------



## Machine Learning Coursework Materials for Samsung DS<sup>2</sup> School 

This repository contains Python code for a selection of tables, figures and LAB sections from the book <A target="_blank" href='http://www-bcf.usc.edu/%7Egareth/ISL/index.html'>'An Introduction to Statistical Learning with Applications in R'</A> by James, Witten, Hastie, Tibshirani (2013).<P>

### Prerequisites
  * [Anaconda](https://www.anaconda.com/download/)
  * [Graphviz](https://graphviz.gitlab.io/download/)
    * [For windows](https://graphviz.gitlab.io/_pages/Download/windows/graphviz-2.38.msi)
      * You should append the bin folder of graphviz in your PATH. (e.g. C:\Program Files (x86)\Graphviz2.38\bin) 
      * See [how to add PATH](http://inforyou.tistory.com/20)
      * *Rebooting may be required to affect the path update.*

### Installation

#### For windows 10 users
 * With anaconda navigator (GUI application)
   * Launch Anaconda navigator with 'Adiminister' privilege.
   * Click 'Environments' tab in the left panel.
   * Select 'Create' button in the bottom of the middle panel.
     * Set Environment name as you wish 
     * In here, I choosed 'ds2'. (You should remember this environment name for future use.)
     * Select the Python version to **3.6** or **2.7**. 
     * Select 'Create' bottom to create a new environment.
   * You should install following packages: 
     - pandas
     - numpy
     - scipy
     - scikit-learn
     - jupyter
     - statsmodels
     - patsy
     - matplotlib
     - seaborn
     - xlrd
   * After choosing 'All' in the dropdown list of the toolbar, you can search the package using search bar. Check out all above and click **Apply** button to install.
   * After all packages have been installed, click 'play icon' of the environment and select 'Open Terminal'
   * Execute the following command to install an additional package.
```   
(ds2)prompt$ pip install pydot
```   

#### For linux users
   * Create a new conda environment as follow (in case of the environment name is ds2):
```
prompt$ conda create -n ds2 python=3.6 pandas numpy scipy scikit-learn jupyter statsmodels patsy matplotlib seaborn xlrd
```
   * After installation finished, activate your environment:
```
prompt$ source activate ds2
```
   * Install the extra package 
     * Check your prompt whether environment is properly changed or not.)   
     * Execute the following command to install an additional package.
```   
(ds2)prompt$ conda install -c conda-forge glmnet
(ds2)prompt$ pip install pydot
```

### Download repository
  * You can download or clone the jupyter notebooks from github (*To Be Updated for students*)
  * I recommend to save or clone files under *Documents* folder.
  
### Launch jupyter notebook
  * If you installed with anaconda navigator, 
    * Go to Home menu and select your environment.
    * Click **'launch'** of jupyter notebook
  * If you installed on linux, type *'jupyter notebook'* in the prompt. 

### Contents of ISLR Folder


<IMG src='http://www-bcf.usc.edu/%7Egareth/ISL/ISL%20Cover%202.jpg' height=20% width=20%> <P>
Chapter 3 - Linear Regression<BR>
Chapter 4 - Classification<BR>
Chapter 5 - Resampling Methods<BR>
Chapter 6 - Linear Model Selection and Regularization<BR>
Chapter 7 - Moving Beyond Linearity<BR>
Chapter 8 - Tree-Based Methods<BR>
Chapter 9 - Support Vector Machines<BR>
Chapter 10 - Unsupervised Learning<P>

This great book gives a thorough introduction to the field of Statistical/Machine Learning. The book is available for download (see link below), but I think this is one of those books that is definitely worth buying. The book contains sections with applications in R based on public datasets available for download or which are part of the <A target="_blank" href="https://cran.r-project.org/web/packages/ISLR/index.html">R-package ISLR</A>. Furthermore, there is a Stanford University online course based on this book and taught by the authors (See <A target="_blank" href='https://lagunita.stanford.edu/courses/'>course catalogue</A> for current schedule).<P>

#### References: 
James, G., Witten, D., Hastie, T., Tibshirani, R. (2013). <I>An Introduction to Statistical Learning with Applications in  R</I>,  Springer Science+Business Media, New York.
http://www-bcf.usc.edu/~gareth/ISL/index.html

Hastie, T., Tibshirani, R., Friedman, J. (2009). <I>Elements of Statistical Learning</I>, Second Edition, Springer Science+Business Media, New York.
http://statweb.stanford.edu/~tibs/ElemStatLearn/