SOURCE_FILES := $(wildcard sources/*.md)

OUTPUT_NAME=master
OUTPUT_DIRECTORY=compiled

clean:
	rm $(OUTPUT_DIRECTORY)/*
pdf:
	pandoc $(SOURCE_FILES) -o $(OUTPUT_DIRECTORY)/$(OUTPUT_NAME).$@
beamer:
	pandoc $(SOURCE_FILES) -t beamer -o $(OUTPUT_DIRECTORY)/$(OUTPUT_NAME).$@.pdf
md:
	pandoc $(SOURCE_FILES) -o $(OUTPUT_DIRECTORY)/$(OUTPUT_NAME).$@
html:
	pandoc $(SOURCE_FILES) -t revealjs -s -o $(OUTPUT_DIRECTORY)/$(OUTPUT_NAME).$@

all : pdf beamer md html

rebuild : clean all
