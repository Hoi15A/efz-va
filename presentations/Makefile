SOURCE_FILES := $(sort $(wildcard sources/*.md))

OUTPUT_NAME=master
OUTPUT_DIRECTORY=compiled

all : pdf beamer md html

pdf:
	pandoc $(SOURCE_FILES) -o $(OUTPUT_DIRECTORY)/$(OUTPUT_NAME).$@
beamer:
	pandoc $(SOURCE_FILES) -t beamer -o $(OUTPUT_DIRECTORY)/$(OUTPUT_NAME).$@.pdf
md:
	pandoc $(SOURCE_FILES) -o $(OUTPUT_DIRECTORY)/$(OUTPUT_NAME).$@
html:
	pandoc $(SOURCE_FILES) -t revealjs -s -o $(OUTPUT_DIRECTORY)/$(OUTPUT_NAME).$@

clean:
	rm $(OUTPUT_DIRECTORY)/*

rebuild : clean all
