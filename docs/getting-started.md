# Installation

Install the CLI with the following command:

```bash
pip install -U smartloop

```

The Command Line Interface allows you upload, fine-tune and extract information from your documents with a few easy steps


## Configuration

Once you have your CLI installed , configure it by running the folloiwng comnand:

```
┌──(smrtlp㉿lexic)-[~]                                                                                        25ms  
└─$ smartloop login
                              _    _
 ___  _ __ ___    __ _  _ __ | |_ | |  ___    ___   _ __
/ __|| '_ ` _ \  / _` || '__|| __|| | / _ \  / _ \ | '_ \
\__ \| | | | | || (_| || |   | |_ | || (_) || (_) || |_) | _
|___/|_| |_| |_| \__,_||_|    \__||_| \___/  \___/ | .__/ (_)
                                                   |_|

Please copy your access token using the link https://dashboard.smartloop.ai/developer
You will need to complete your authentication process to obtain / generate access token
Paste your token (Token will be invisible):


```

This will take you through the process of creating a [free account](https://app.smartloop.ai/signup).


## Create a Project

This is the top-level grouping where all your contents and model is configured at a project level:

```
smartloop projects create --name microsoft
```

## Upload Document


Once the project is selected , upload documents from your folder or a specific file to personalized your project, in this case I am uploading the a document describing Microsoft online services form my local machine:

```
smartloop upload --path=~/document1.pdf
```

## Prompting

You can start prompting by executing the following commnand:

```
smartloop run
```

This will start the interactive interface that will let you interact with the model against your uploaded document(s)


Below is an example of the interactive interface:

```
Microsoft(microsoft-24-07-2024)
======================================
Enter prompt (Ctrl-C to exit): 
what the SLA for azure open ai
⠋
The SLA (Service Level Agreement) for Azure OpenAI is not explicitly mentioned in the provided text. However, it's possible that the SLA for Azure OpenAI might be similar to the one mentioned below:

"Uptime Percentage"

* Service Credit:
+ < 99.9%: 10%
+ < 99%: 25%
+ < 95%: 100%

Please note that this is not a direct quote from the provided text, but rather an inference based on the format and structure of the SLA mentioned for other Azure services (e.g., SAP HANA on Azure High Availability Pair). To confirm the actual SLA for Azure OpenAI, you should check the official Microsoft documentation or contact their support team.

Prompt message (Ctrl-C to exit):
```


