This directory contains the necessary scripts to generate Mac OSX Dictionary from Rails 2.3 source code.

## Building dictionary

Generate Rdoc from Rails source to ``doc/rdoc`` directory and run Ruby script included in this package to generate xml file that will be used to generate dictionary

    rdoc <RAILS_SOURCE_DIR>
    ruby ./dictionary_generator.rb

Build dictionary contents from generated xml file

    make all

Install dictionary to your ``~/Library/Dictionaries`` directory

    make install
