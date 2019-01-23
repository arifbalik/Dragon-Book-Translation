# Dragon-Book-Translation
This is a translation project of the book *Compilers : Principles, Techniques, & Tools* (a.k.a. Dragon Book) to Turkish with a deadline to the end of 2019.

# Contribution
- Every pull request should include *spent time* info in its summary. For example;

  ``` Some commit [30min] ```

  that is how much time spent to translate a section, equation, figure or fixing a bug.

- Also chapters, sections, figures, equations etc. should be included in main tex file as seperate files with using `\input` command. For example when including a chapter;

  ``` 
  .
  .
  .

  \input{preface/preface}
  \input{contents/contents}

  \input{chapters/chapterX/[your-chapter-file.tex]}

  ```

  And in every chapter;
  ``` 

  Some text...

  \input{figures/fig_[your-figure.tex]}
  \input{equations/eq_[your-equation.tex]}

  Some more text...

  ```
