# Created by mbenlioglu

# Project setup

project(CV-resume NONE)
cmake_minimum_required(VERSION 3.10)

set(PDFLATEX_COMPILER pdflatex)

include(cmake/UseLATEX.cmake)

# Outputs
add_latex_document(full-pr.tex
            TARGET_NAME full-prof
            INPUTS functions.tex
#            BIBFILES publications.bib
            )
#add_latex_document(full-ac.tex
#            TARGET_NAME full-ac
#            INPUTS functions.tex
#            BIBFILES publications.bib
#            )
#add_latex_document(resume.tex
#            TARGET_NAME resume
#            INPUTS functions.tex
#            BIBFILES publications.bib
#            )
