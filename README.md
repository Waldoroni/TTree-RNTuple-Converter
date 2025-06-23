#[ROOT] TTree-to-RNTuple Converter
This program is takes in a ROOT data file and converts any TTree found in the file into an RNTuple, using ROOT's RNTuple Importer, currating the TTree to be able to be sent through the RNTuple importer. 

Another program that is included in this repo is a program that checks to see if the two corresponding files are usable for the program, ensuring that the importer has done its job.

These programs were made in light of the upcoming ROOT 7 update, which will now use RNTuples as the main form of data storage, instead of TTrees. This program will allow for the conversion from multiple TTrees into RNTuples, while maintaining the data of the previous file. 

In the future, we hope to expand upon our "checker" program, as currently, checking each individual column of an TTree and making sure that the corresponding RNTuple is exactly the same. 

Furthermore, we hope continue our work on the importer, allowing for the transfer of certain objects such as TH1 objects into an RNTuple. This comes from the inclusion of a new histogram class that will be implemented in ROOT 7.