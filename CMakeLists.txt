# Created by mbenlioglu
cmake_minimum_required(VERSION 3.14)

# Add UseLATEX v2.7.2
include(FetchContent)
FetchContent_Declare(
    UseLATEX
    URL https://gitlab.kitware.com/kmorel/UseLATEX/-/raw/Version2.7.2/UseLATEX.cmake
    DOWNLOAD_NO_EXTRACT TRUE
)
FetchContent_MakeAvailable(UseLATEX)
include(${uselatex_SOURCE_DIR}/UseLATEX.cmake)

# Project setup
project(CV-resume NONE)

set(PDFLATEX_COMPILER pdflatex)

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
