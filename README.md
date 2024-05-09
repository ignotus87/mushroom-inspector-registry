# mushroom-inspector-registry
Parsed form of the Government Office's registry Excel file containing the data of all Hungarian mushroom inspectors

# source file
The original input file is always included in OriginalInput\Latest. The old ones are in OriginalInput\History.L

Unfortunately, the latest input files are provided in pdf format.

It can be downloaded from ever-changing locations 
This actual one is from [this location at the Pest County Government Office server](https://www.kormanyhivatal.hu/hu/pest/szervezeti-egysegek-elerhetosegei/elelmiszerlanc-biztonsag-foldhivatali-noveny-es-talajvedelmi-erdeszeti-foosztaly/felugyeleti-osztaly).

You can find the ever latest version [with this Google search](https://www.google.com/search?q=kormanyhivatal+gombaszakellen%C5%91r%C3%B6k+list%C3%A1ja)
The first result will be the latest Excel file.
After donwload, it must be saved as .xlsx in order to be processable as xml.

# processing
First, the input pdf has to be converted to xlsx.
Use this free online converter: [SmallPdf](https://smallpdf.com/pdf-to-excel#r=result&t=1d5a38bd911c2fc8e1f379e4902b90f3&i=convert-to-excel)
It generates a multi-sheet pdf.
The sheets need to have the same schema, last time I had to move all data from Table4 and 5 to Table3 
in order to be further processable.

The xlsx file is then processed using [Alteryx Designer](https://www.alteryx.com/). 
Unfortunately it is a non-open-source data processing workflow tool.
You can view and test the .yxmd workflow if you donwload the trial.
If you don't want to, you can still have a look at the workflow by inspecting
this snapshot:

![Alteryx Workflow Snapshot](./Alteryx/AlteryxWorkflow.png)

The outputs are located under the folder Output.
These are to be kept up-to-date so you can use them as a data source.

# contact if
If you need other file formats feel free to ask.

Also, if you find any bugs/missing data, post a message/issue.
