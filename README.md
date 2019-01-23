# Dragon-Book-Translation
This is a translation project of the book *Compilers : Principles, Techniques, & Tools* (a.k.a. Dragon Book) to Turkish with a deadline to the end of 2019.

# Folder Structure

Every chapter, figure, equation and anything that is not a pure text and more than couple of lines should be written as a sepetare tex file. 

Project has some main catagories;
```
Book

  --main_file.tex
  --chapters
    --chapter1.tex
    --chapter2.tex
    --chapterX.tex
    --...
  --figures
    --fig1_1.tex
    --fig4_7.tex
    --fig[section_no]\_[no].tex
    --...
  --equations
    --eq1_1.tex
    --eq1_2.tex
    --eq[no].tex
    --...
  --preface
    --preface.tex
    --preface_of_translator.tex
    --...
  --contents
    --list_of_figures.tex
    --contents.tex
    --...
  --appendix
    --appendix_a.tex
    --appendix_X.tex
    --...
  --custom_category
    --custom_file.tex
    --...

```


# Contribution
- **Every pull-request should have *spent time* info in its summary (unless not specified in tex file or negligible).** For example;

  ``` Some commit [30min] ```

  that is how much time spent to fixing a bug or doing some other thing than directly translating the book.
  
- **Every section and subsection should have spent time with its name;**
  ```tex 
  \section{Chapter Name [30min]}
  ```
  This is only for the text and not for figures, equations etc. You can give them in pull-request decription or in tex file;
  ```tex 
  %[10min]
  \begin{equation}
    ...
  \end{equation}
  ```

- **Also chapters, sections, figures, equations etc. should be included in main tex file as seperate files with using `\input` command.** For example when including a chapter;

  ```tex
  .
  .
  .

  \input{preface/preface}
  \input{contents/contents}

  \input{chapters/chapterX/[your-chapter-file.tex]}

  ```

  And in every chapter;
  ```tex 

  Some text...

  \input{figures/fig_[your-figure.tex]}
  \input{equations/eq_[your-equation.tex]}

  Some more text...

  ```
- **Please be spesific about descriptions both in pull-requests and issues.**

# Contributors

- Arif Balik
