# mushroom-inspector-registry
Parsed form of the Government Office's registry Excel file containing the data of all Hungarian mushroom inspectors

# source file
The original input file is always included in OriginalInput\Latest. The old ones are in OriginalInput\History
It is downloaded from [this location at the Government Office server](https://www.kormanyhivatal.hu/download/c/5f/16000/GOMBA-szakellen%C5%91r%20NYILV%C3%81NTART%C3%81S_202006.xlsx).

You can find the ever latest version [with this Google search](https://www.google.com/search?q=kormanyhivatal+gombaszakellen%C5%91r%C3%B6k+list%C3%A1ja)
The first result will be the latest Excel file.
After donwload, it must be saved as .xlsx in order to be processable as xml.

# processing
The input file is processed using [Alteryx Designer](https://www.alteryx.com/). 
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
