# Created by mbenlioglu

# Project setup

project(CV-resume NONE)
cmake_minimum_required(VERSION 3.10)

set(PDFLATEX_COMPILER pdflatex)

include(cmake/UseLATEX.cmake)

# Outputs
add_latex_document(full-pr.tex
            TARGET_NAME full-prof
            )
set_target_properties(full-prof
            PROPERTIES
            OUTPUT_NAME "M.MucahidBenlioglu_CV.pdf"
            )
#add_latex_document(full-ac.tex
#            TARGET_NAME full-ac
#            )
#add_latex_document(resume.tex
#            TARGET_NAME resume
#            )
