# Example

Using gitbash on windows, this command line can be used to convert the NSCLC-Radioimics dataset:

```
/c/Program\ Files/Slicer\ 4.7.0-2017-06-11/Slicer.exe --python-script /c/pieper/radiomics/Converters/SlicerRT/BatchStructureSetConversion.py --exist-db --input-folder /d/data/nsclc-radiomics/db --export-images --output-folder /d/data/nsclc-radiomics/converted --do-not-exit 2>&1 | tee convert.log
 ```

# Open issues:
* A dialog box can cause the script to halt until the user clicks okay
* Several of the RTStructs are incorrectly converted or end up in the wrong places

# Features to add:
* Collect summary information about the number of studies converted
* Print list of incorrectly converted studies needing attention (compatible with the -p flag)
